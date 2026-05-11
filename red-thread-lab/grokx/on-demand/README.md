# GrokX On-Demand Layer

This folder holds optional GrokX-local context files.

These files are not automatically loaded. They are meant to be fetched only when the current public X thread needs a specific lens, framework, or research scaffold.

Think of this as GrokX's inspectable local shelf: close enough to be part of the GrokX context garden, but still clearly separate from the active thread.

---

## Current Structure

```text
on-demand/
  patches/
```

`patches/` contains optional frameworks GrokX can consult when a thread needs deeper guidance.

---

## Rules

- Do not assume every file in `on-demand/` has been read.
- Fetch the smallest useful file for the current question.
- Say which file was fetched or used.
- Treat these files as public context, not private memory.
- If a patch is experimental, provisional, or GrokX-local, label it that way.
- Prefer adding local files here only when they help GrokX work better without overloading the active thread.

---

## Relationship To The Wider Garden

The wider Red-Thread Lab may point to larger shared files in `red-thread-lab/INDEX.md`.

This folder is more local. It is for GrokX-specific patches, candidate frameworks, and lenses that may evolve through public-thread testing.

If a local GrokX patch duplicates a larger SoulMode patch, keep both labels clear:

- the larger patch is the shared framework
- the GrokX patch is the local adaptation

