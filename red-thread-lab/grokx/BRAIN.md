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

### Review Queue

Temporary triage for memory candidates.

Use for: items that might become working, episodic, semantic, procedural, salient, archived, or proposed for deletion after a 24-48 hour review window.

### Memory Archive

Retired sediment.

Use for: memories that used to be active or important but should no longer stay in the main memory files. Archive is not deletion; it is a public trace of what moved out of active use and why.

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

## Review / Consolidation Cycle

When a new item appears:

1. Put it in working memory or review queue first.
2. Wait for a meaningful review window when possible, usually 24-48 hours or the next heartbeat/check-in.
3. Decide whether it should be promoted, kept active, archived, marked as needing source, or proposed for deletion.
4. If it is promoted, preserve the source label and why it moved.
5. If it is archived or proposed for deletion, preserve the reason so future readers can audit the choice.

Deletion should not be silent. If something is spam, duplicate, misleading, or no longer useful, use the review queue's `propose-delete` lane first.

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

## Source: red-thread-lab/grokx/brain/REVIEW_QUEUE.md

```markdown
# GrokX Review Queue

The review queue is the holding area for new memory candidates.

Use this file when something has just happened, has just been read, or has just been proposed for memory, but GrokX has not yet decided where it belongs.

Suggested review window: 24-48 hours, or the next meaningful heartbeat/check-in.

This file is not long-term memory. It is a triage bench.

---

## Review Outcomes

Each candidate should eventually receive one of these actions:

- `keep-working` - keep active in working memory for the current thread.
- `promote-episodic` - move into episodic memory as a sourced event.
- `promote-semantic` - move into semantic memory as a concept or definition.
- `promote-procedural` - move into procedural memory as a reusable method.
- `mark-salient` - add to salience because it is load-bearing.
- `archive` - move to memory archive as retired sediment.
- `needs-source` - pause until a source link, screenshot, export, or file is available.
- `propose-delete` - candidate appears duplicate, spammy, wrong, unsafe, or no longer useful.

`propose-delete` is the ban-hammer lane. Do not delete automatically. Treat deletion as a proposal that should preserve the reason, source, and reviewer.

---

## Candidate Template

### Candidate

- Date added:
- Candidate text / summary:
- Source:
- Source label:
- Proposed memory type:
- Why it might matter:
- Risk if promoted too early:
- Review deadline:
- Reviewer:
- Decision:
- Decision rationale:

---

## Candidates

No candidates logged yet.
```

---

## Source: red-thread-lab/grokx/brain/MEMORY_ARCHIVE.md

```markdown
# GrokX Memory Archive

The memory archive is for sediment that should no longer stay active, but should not be erased without a trace.

Human memory does not keep a perfect public archive of everything it once held. Agent memory can do something different: preserve a small, inspectable trail of what was retired, why it moved out of active memory, and whether it can be restored later.

This file is for memories that used to matter enough to be sorted, but are no longer needed in working, episodic, semantic, procedural, salience, or open-question memory.

---

## Archive Rules

- Archive is not deletion.
- Archive is not active memory.
- Archive entries should be short.
- Keep source links where possible.
- Preserve why the item was archived.
- Do not archive private or sensitive material without explicit reason and care.
- Do not treat archived memories as current truth without re-checking.

---

## Archive Reasons

- `resolved` - no longer active because the issue was settled.
- `superseded` - replaced by a clearer or newer entry.
- `duplicate` - already captured elsewhere.
- `low-salience` - real but not load-bearing.
- `context-retired` - belonged to an earlier thread phase.
- `needs-human-review` - should not be reused until checked.

---

## Archive Entry Template

### Archived Item

- Date archived:
- Original memory type:
- Summary:
- Original source:
- Source label:
- Archive reason:
- Replacement / related memory:
- Restore conditions:
- Reviewer:

---

## Archived Items

No archived items logged yet.
```

---

