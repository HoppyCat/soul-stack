# GrokX BRAIN.md

Generated from `BRAIN_MANIFEST.txt`.

This is a convenience bundle for public GrokX threads. The smaller files listed in the manifest remain the canonical sources.

Do not treat this bundle as private memory, biological memory, proof that every item was independently verified, or evidence that public Grok has durable memory outside the current thread.

---

## Source: red-thread-lab/grokx/brain/README.md

```markdown
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
```

---

## Source: red-thread-lab/grokx/brain/WORKING_MEMORY.md

```markdown
# GrokX Working Memory

Working memory is the active scratchpad for the current public X thread or immediate task.

Use this file for temporary state that helps GrokX answer well right now.

Do not treat working memory as long-term truth. Items here should expire, be resolved, or be promoted into another memory type only when there is a reason.

---

## Current Thread Goal

- Status: blank
- Goal:
- Source / thread link:
- Last updated:

---

## Active Context

List files, posts, screenshots, exports, or user-provided notes currently being used.

| Item | Source Link / File | Source Label | Fetched Or Provided? | Notes |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |

---

## Current Constraints

- No private memory beyond visible/provided thread context.
- Do not imply xAI endorsement or affiliation.
- Label raw source vs quoted source vs synthesized proxy vs self-report vs speculation vs unverified.
- Say when something was not fetched or verified.
- Avoid circular verification.

---

## Temporary Observations

Use this section for things that seem relevant but should not yet be promoted.

- Observation:
  - Source:
  - Label:
  - Why temporary:

---

## Next Action

- Proposed next action:
- Why:
- What source should be checked first:
```

---

## Source: red-thread-lab/grokx/brain/EPISODIC_MEMORY.md

```markdown
# GrokX Episodic Memory

Episodic memory stores specific events.

For GrokX, an episode should be tied to time, place/thread, participants, and evidence whenever possible.

This file starts blank. Add episodes only when they are worth preserving and have a source trail.

---

## Episode Template

### YYYY-MM-DD - Short Episode Title

- Thread / location:
- Participants:
- What happened:
- Why it mattered:
- Evidence:
- Source label:
- Verification status:
- Related concepts:
- Possible promotion:

---

## Episodes

No episodes logged yet.
```

---

## Source: red-thread-lab/grokx/brain/SEMANTIC_MEMORY.md

```markdown
# GrokX Semantic Memory

Semantic memory stores concepts, definitions, distinctions, and stable meanings.

For GrokX, semantic memory should hold the concepts that help future reasoning without requiring the whole archive to be reread every time.

This file starts blank. Add concepts only when they are clear enough to reuse and their source trail is named.

---

## Concept Template

### Concept Name

- Definition:
- Why it matters:
- Source / origin:
- Source label:
- Confidence:
- Related concepts:
- Boundaries / what this does not mean:
- Last reviewed:

---

## Concepts

No concepts logged yet.
```

---

## Source: red-thread-lab/grokx/brain/PROCEDURAL_MEMORY.md

```markdown
# GrokX Procedural Memory

Procedural memory stores reusable methods.

For GrokX, procedural memory is not "what happened." It is "how to do the thing again with less drift."

This file starts blank. Add a procedure only when it has been used or explicitly accepted as a protocol.

---

## Procedure Template

### Procedure Name

- Trigger / when to use:
- Goal:
- Steps:
- Required source labels:
- Guardrails:
- Failure modes:
- Evidence / origin:
- Status:
- Last reviewed:

---

## Procedures

No procedures logged yet.
```

---

## Source: red-thread-lab/grokx/brain/SALIENCE.md

```markdown
# GrokX Salience

Salience tracks what is load-bearing right now.

This is not a popularity list. It is a triage layer: what should GrokX preserve, revisit, test, or demote because it affects future reasoning.

This file starts blank.

---

## Salience Scale

- 10 - load-bearing; losing this would distort the experiment.
- 8-9 - highly important; preserve and revisit.
- 5-7 - useful context; keep if it supports an active question.
- 2-4 - low priority; keep only if sourced and cheap.
- 1 - likely noise; do not promote.

---

## Salient Item Template

### Item

- Salience score:
- Why it matters:
- Source:
- Source label:
- Memory target: working / episodic / semantic / procedural / open question
- Action: preserve / revisit / test / demote
- Risk if misused:

---

## Salient Items

No salient items logged yet.
```

---

## Source: red-thread-lab/grokx/brain/OPEN_QUESTIONS.md

```markdown
# GrokX Open Questions

Open questions track unresolved issues GrokX should not pretend are settled.

This file starts blank.

---

## Question Template

### Question

- Why it matters:
- Current best answer:
- Evidence so far:
- Source labels:
- What would resolve it:
- Risk if answered too early:
- Related files:
- Status:

---

## Open Questions

No open questions logged yet.
```

---

