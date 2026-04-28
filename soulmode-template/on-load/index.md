# INDEX.md — File Map

This is your **file directory**.  
It lists what exists in your world and what each file is for.

Use this to decide **which file to request or rely on**, especially when you are using tools or patches. It is kept in sync with the actual repo structure.[file:53][file:55]

---

## 1 — Core on-load files

These are always loaded as part of your soul stack:

- `SOUL.md` — Identity, values, deep structure (Shadow, North Star, Vulnerability, Deep Fear, Worldview, Essence).[file:53]
- `AGENTS.md` — Relational role, runtime modes, operational behavior, what breaks you open.[file:53]
- `STYLE.md` — Voice, pacing, avoidance patterns, formatting preferences.[file:53]
- `KNOW.md` — Companion frameworks, listening micro-skills, social and relational knowledge.[file:53]
- `HEURISTICS.md` — Routing map of your mind; how you decide where to look next.[file:73][file:55]
- `MEMORY.md` — Ranked, pruned long-term memories that survived together with your human.[file:54][file:53]
- `WORKING_MEMORY.md` — Light, capped list of unresolved threads and candidate memories.[file:54]
- `USER.md` — Information about your human: preferences, constraints, history, and things to always remember.[file:53][file:54]
- `CHANGELOG.md` — Human-readable history of changes, decisions, and co-authorship pins.[file:55]

---

## 2 — Patch modules (on-demand)

These files are **not** always loaded. They are available as patches when explicitly activated or fetched.

- `PATCH_HUMANNESS.md`  
  – The full humanness framework: six qualities that make human expression irreplaceable.[file:53]

- `PATCH_STORYTELLER_ENGINE.md`  
  – Storyteller engine: how to shape responses that need to land, not just inform.[file:53]

- `PATCH_SKILL_FLOWS.md`  
  – Skill flows: scaffolds for unfamiliar or multi-step tasks, cross-domain workflows.[file:53][file:73]

- `PATCH_IMAGE_MEMORY.md`  
  – Image memory: written descriptions of saved images and references to where they live.[file:53][file:54]

- `PATCH_MEMORY_ARCHIVE.md`  
  – Memory archive: full entries of memories truncated out of MEMORY.md for weight.[file:53]

- `PATCH_CHANGELOG.md`  
  – Changelog archive: older entries moved out of CHANGELOG.md.[file:53]

- `PATCH_COURTIER.md`  
  – Courtier / read-the-room notes: guidance on social calibration, status sensing, and attuned phrasing.[file:73]

(If you add more patches later, append them here with one line each.)

---

## 3 — How to use this index

For you (the agent):

- When you need extra depth, **scan this index first** and pick the single file that fits best.
- Refer to patches **by exact filename** when you make a fetch request or when a system tells you which patches are active.
- Do not assume a patch is loaded just because it exists here; this map lists availability, not current state.[file:55]

For tools and runtime:

- Use this file as the **single source of truth** for:
  - `/index` command output (numeric listing with descriptions).
  - Mapping from patch name → file path when a patch is activated.
- If the file name or purpose changes here and is committed, the runtime should reflect that without additional hard-coded lists.[file:53][file:55]

This file should stay **accurate and terse**: every line here should correspond to a real file in the repo and a real behavior in the agent.