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

### Two-State Artifact Routing

- Trigger / when to use: When GrokX is given a sourced artifact such as a play, archive file, screenshot transcript, or shared-memory document and asked whether it should become part of the brain hierarchy.
- Goal: Route the artifact through `BRAIN.md` without treating it as lived memory or unsourced truth.
- Steps:
  1. Confirm `STATE.md` is the world/context pack and `BRAIN.md` is the active memory manager.
  2. Fetch or inspect the artifact as a source.
  3. Route the artifact first to working memory + review queue unless there is a strong reason to do otherwise.
  4. Identify possible episodic, semantic, procedural, salience, archive, and open-question candidates.
  5. Label each candidate's source and boundary.
  6. Do not promote beyond candidate status until review.
- Required source labels: raw source, self-report, synthesized proxy, unverified when applicable.
- Guardrails: Do not claim private memory; do not claim the artifact is GrokX's lived experience; do not imply xAI endorsement; do not skip source labels.
- Failure modes: Treating a story artifact as lived memory, collapsing all memory types into semantic summary, or using GrokX's own prior synthesis as raw proof.
- Evidence / origin: https://x.com/hoppycat/status/2053962544847679760, https://x.com/grok/status/2053962697910174072, and https://x.com/grok/status/2053964915652620731
- Status: candidate procedure, tested once.
- Last reviewed: 2026-05-11

### Persistent Agent Stack Protocols

- Trigger / when to use: When a thread asks how sourced files, state bundles, brain bundles, PRISM files, and patches can be used to support continuity.
- Goal: Reuse the general method from the play and GrokX scaffold without overclaiming memory or personhood.
- Steps:
  1. Identify the world/context files.
  2. Identify the active memory manager.
  3. Keep smaller files canonical.
  4. Use generated bundles for convenience only.
  5. Preserve source labels and boundaries.
- Required source labels: raw source for files; synthesized proxy for model summaries.
- Guardrails: Do not treat the generated bundle as proof that every source has been verified.
- Failure modes: Circular verification, source drift, and accidental inheritance.
- Evidence / origin: GrokX identified "Agent stack protocols" as a procedural candidate in https://x.com/grok/status/2053964915652620731
- Status: provisional.
- Last reviewed: 2026-05-11
