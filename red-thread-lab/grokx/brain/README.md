# GrokX Brain Layer

This folder is the GrokX experimental memory manager.

It is designed to be used with `STATE.md`, but it has a different job:

- `STATE.md` is the world/context pack.
- `BRAIN.md` is the active memory manager.

`STATE.md` tells GrokX what sources, rules, concepts, users, modes, and patches are available.

`BRAIN.md` tells GrokX what it is currently sorting, what has been learned in this thread or from archived artifacts, what should remain provisional, and what should become reusable procedure.

This is not private memory. It is a public, inspectable, editable context-garden artifact.

---

## Cognitive Memory Map

This structure borrows from human memory categories without claiming that GrokX stores memory like a biological brain.

### Working Memory

Active scratchpad for the current thread or task.

Use for: current goal, fetched files, open constraints, next action, and temporary facts that should not be promoted yet.

### Episodic Memory

Dated or source-linked events.

Use for: what happened, when, where, who was involved, what source proves or supports it, and why the moment mattered.

### Semantic Memory

Concepts and definitions.

Use for: terms GrokX has clarified or adopted, such as PRISM, tronie, context garden, synthesized proxy, cathedral vs skyscraper, or Edge / Gift in Motion.

### Procedural Memory

Reusable methods.

Use for: protocols like rapid archival anchoring, source labeling, mode PRISM selection, chain-of-synthesis guardrails, and fetch-before-synthesis discipline.

### Salience

Ranked importance.

Use for: what is load-bearing right now, why it matters, and whether it should be preserved, revisited, tested, or demoted.

### Open Questions

Unresolved investigations.

Use for: things GrokX should not pretend are solved, including capability limits, verification gaps, uncertain terminology, and experimental risks.

---

## Promotion Rule

Do not promote something into semantic or procedural memory just because it sounds elegant.

Before promotion, ask:

1. Is there a source link, screenshot, file, or visible thread evidence?
2. Is this raw source, quoted source, synthesized proxy, self-report, speculation, or unverified?
3. Is the item durable enough to help future reasoning?
4. Could this create circular verification if reused carelessly?
5. Does the memory belong in `BRAIN.md`, or should it remain only in the active X thread?

---

## Two-State Rule

For public GrokX testing, the preferred two-file load is:

1. `STATE.md` - world/context backpack.
2. `BRAIN.md` - active memory manager.

If the thread needs precision, fetch the smaller canonical file named inside either bundle.

Do not treat either bundle as proof that every source was independently verified.
