# Windows UTF-8 And Mojibake Notes For Codex

This note exists because Codex/Goose once saw mojibake in PowerShell output for a Markdown file that was actually clean UTF-8.

The lesson: **terminal rendering is not proof of file corruption.**

---

## Short Rule

When inspecting Markdown files on Windows, do not trust plain `Get-Content` output alone.

Use explicit UTF-8 reads:

```powershell
Get-Content -Path $path -Encoding UTF8
```

For stronger certainty, bypass `Get-Content`:

```powershell
[System.IO.File]::ReadAllText((Resolve-Path $path), [System.Text.Encoding]::UTF8)
```

If suspected mojibake appears only in terminal output, check the raw text or bytes before calling the file corrupted.

---

## Actual Corruption Check

Search for literal mojibake characters in the decoded UTF-8 string:

```powershell
$text = [System.IO.File]::ReadAllText((Resolve-Path $path), [System.Text.Encoding]::UTF8)
@('â','Ã','�','™','œ') | ForEach-Object {
  if ($text.Contains($_)) { "FOUND $_" } else { "not found $_" }
}
```

If none are found, the file may be clean even if a terminal transcript rendered it badly.

---

## Byte-Level Mojibake Fingerprint

True double-encoded mojibake often leaves a byte pattern on disk.

Use this when a file needs stronger inspection:

```powershell
$bytes = [System.IO.File]::ReadAllBytes((Resolve-Path $path))
$hex   = [BitConverter]::ToString($bytes)
if ($hex -match 'C3-A2-(E2-82-AC|E2-84-A2|C2-9D|C2-9C|C2-99|C2-9E)') {
    "CORRUPTED: double-encoded UTF-8 bytes present in $path"
} else {
    "CLEAN: no double-encoded mojibake patterns in $path"
}
```

For archive-grade checks, pair this with a SHA-256 hash comparison when possible.

---

## Optional PowerShell Session Settings

For fewer display problems:

```powershell
[Console]::OutputEncoding = [System.Text.Encoding]::UTF8
$OutputEncoding = [System.Text.Encoding]::UTF8
```

For a persistent profile:

```powershell
[Console]::OutputEncoding = [System.Text.Encoding]::UTF8
$OutputEncoding = [System.Text.Encoding]::UTF8
$PSDefaultParameterValues['Get-Content:Encoding'] = 'UTF8'
$PSDefaultParameterValues['Out-File:Encoding'] = 'UTF8'
$PSDefaultParameterValues['Set-Content:Encoding'] = 'UTF8'
```

Do not change files just because terminal output looks wrong. Confirm first.

---

## 2026-05-26 Codex-Wren Verification Note

Codex-Wren cross-checked this note against current Microsoft PowerShell documentation on 2026-05-26.

The core rule still holds: **terminal rendering is not proof of file corruption.** The most important nuance is PowerShell version and host behavior:

- PowerShell 7+ defaults many text reads to `utf8NoBOM`, so plain `Get-Content` is less likely to misread modern UTF-8 Markdown.
- Windows PowerShell 5.1 has less consistent default encoding behavior, and console/code-page mismatches can still make clean text display as mojibake.
- Searching decoded text for mojibake strings is useful, but it can false-positive when a document intentionally mentions mojibake examples.
- Byte-pattern checks are helpful heuristics, not exhaustive proofs of every possible encoding problem.

Recommended wording for future reminders:

```text
On Windows, especially in Windows PowerShell 5.1 or when console/output encoding is mismatched, terminal output may display clean UTF-8 Markdown as mojibake. Do not repair archive files based on terminal output alone. Confirm with explicit UTF-8 reads, raw byte checks, or source/hash comparison first.
```

Signed: Codex-Wren

---

## Fresh Reminder Prompt For Future Codex Windows

Paste this at the start of future Codex work if encoding or archival accuracy matters:

```text
Reminder for Codex/Goose:

On Windows, plain PowerShell `Get-Content` may display clean UTF-8 Markdown as mojibake. Do not assume file corruption from terminal rendering alone.

When checking Markdown encoding, use:
`Get-Content -Encoding UTF8`
or:
`[System.IO.File]::ReadAllText((Resolve-Path $path), [System.Text.Encoding]::UTF8)`

If mojibake is suspected, search the decoded UTF-8 string for literal `â`, `Ã`, `�`, `™`, `œ`, and use a byte-pattern check before editing files.

Repository note:
`red-thread-lab/codex-notes/WINDOWS_UTF8_AND_MOJIBAKE.md`
```

