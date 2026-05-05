# Shared Context Garden Experiment

This experiment tests whether several LLMs can be given a small shared memory surface without requiring a full custom runtime.

The user gives each LLM the same lightweight `HEURISTICS.md` document. That document points to a small root index. The root index points to named shard indexes. Each shard points to public Markdown files in this repo.

The goal is not to prove that the architecture works at scale yet. The goal is to test whether a lightweight, manually pasted routing layer can help different LLMs navigate the same public archive with less repeated explanation.

## Test Shape

1. Ask the LLM a baseline question with only normal chat context, the SoulMode README, and the play if desired.
2. Save the answer.
3. Paste `HEURISTICS.md`.
4. Ask the same or related question and allow the LLM to retrieve from the linked indexes.
5. Save the answer.
6. Compare whether the shared retrieval surface improves continuity, accuracy, attribution, or relational tone.

## Safety Boundaries

- Use public GitHub files only.
- Do not place private participant-sensitive memory in remote indexes.
- Treat AI system names as research provenance, not company endorsement.
- Keep the first test small. One root index, a few shard indexes, and one or two fetched docs is enough.

## Key Question

Does a small shared context garden make the loop feel more coherent, or does it make each LLM feel more like a search interface?

