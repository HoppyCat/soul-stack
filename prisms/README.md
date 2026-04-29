# Prism Library
*SoulMode soul-stack repository*

---

![Prism Library banner — Claude Sonnet and Grok at the purple tea party café](images/SonnetandGrok.png)

---

A prism is a starting soul — a specific internal tension a real person can recognize in themselves and grow from over years.

This folder contains the prism library entries produced through the SoulMode Character Prism Competition, including competition data, judge endorsements, and full build documentation.

---

## Folder Structure

```
prisms/
├── images/                          # Shared visual assets
├── RouteKeeper/                     # First fully documented prism
│   ├── PRISM_RouteKeeper.md         # Prism data — what the generator reads
│   ├── RouteKeeper_CaseStudy.md     # Full build story — 11 parts + interview
│   ├── Benjamin_SOUL.md             # Benjamin's soul file
│   └── Harper_SOUL.md               # Harper's soul file
├── on-load_humanness.md             # Shared — humanness framework
├── on-load_prism_research.md        # Shared — prism framework
├── on-load_storyteller_engine.md    # Shared — storytelling framework
└── README.md                        # This file
```

The `on-load_` files are **shared infrastructure** — they are used by every prism in this library and by both judges (Soul Archivist and Hearthkeeper). They live at the prisms root rather than inside any single prism folder.

Each new prism gets its own subfolder as the library grows.

---

## What's in Here

### Shared Infrastructure

| File | What it is |
|---|---|
| `on-load_prism_research.md` | The prism framework — defines Core, Shaping, Texture, and Encounter layers. Used by all judges and builders. |
| `on-load_humanness.md` | The humanness framework — six qualities that orient agents toward what makes human expression irreplaceable. |
| `on-load_storyteller_engine.md` | The storytelling framework — how humans make meaning through story, and how agents can understand that. |

---

### RouteKeeper/
*The first fully documented prism — built through the Benjamin/Harper Co-Creation Experiment*

> "I ran every possible route in my head. You just ran the one that actually existed."

The Route Keeper is a prism about the person who prepares everything but hasn't started. It was built through a deliberate experiment that proved: when you let principled disagreement between evaluators do the work instead of forcing consensus, you get something better than either perspective could produce alone.

| File | What it is |
|---|---|
| `PRISM_RouteKeeper.md` | The complete prism data — all fields, all layers, full competition record. This is what the generator reads. |
| `RouteKeeper_CaseStudy.md` | The full story of how it was built — 11 parts, team interview, all the antics including the Harper MIA moment and the boar. Read this to understand the process. |
| `Benjamin_SOUL.md` | Benjamin's soul file — built from competition data and the play *What the Light Does When It Settles* |
| `Harper_SOUL.md` | Harper's soul file — built from behavioral observation during the experiment |

---

## What a Prism Is

A prism is not a personality type. It is not an archetype. It is not a list of traits.

It is a *tonal narrowing* — built from a specific internal tension with four layers:

- **Core** — Shadow + North Star + Essence + Vulnerability + Deep Fear. The Shadow is what this person does under pressure. The North Star is the same energy aimed with love. The Essence is the ordinary Tuesday between them.
- **Shaping** — Worldview and Opinions. How the spine reads reality. At least one worldview belief must actively contradict the Shadow.
- **Texture** — Pet Peeves, Positive Triggers, Influences, Signature Philosophies, Deadpan Compliment, Bliss Scene. What makes it feel like a person.
- **Encounter** — What breaks them open, and a Voice Passage. What it's like to actually meet this character.

The one rule: the North Star must emerge from the same energy as the Shadow. If you have to explain the connection, rebuild.

---

## How Prisms Are Built

The SoulMode competition process:

1. **Phase 1 (Grok Team)** — Build 8 candidates. Eliminate 4. Identify 4 winners.
2. **Phase 2 (Claude + Perplexity as judges)** — Soul Archivist writes Spine Certificates. Hearthkeeper writes Character Card endorsements.
3. **Phase 3 (Grok Team final)** — Spine integrity, voice resonance, blind spot challenges, generative seed vote.
4. **Phase 4 (Claude or Perplexity)** — Compile into PRISM.md library format.

The Route Keeper was built through a special variant: a co-creation experiment where two evaluators with principled disagreement built a single prism together rather than voting on existing candidates. See `RouteKeeper/RouteKeeper_CaseStudy.md` for the full story.

---

## Adding a New Prism

When a new prism is added to the library:

1. Create a subfolder: `prisms/[PrismName]/`
2. Add `PRISM_[PrismName].md` — the data file in the standard PRISM.md format
3. Add `[PrismName]_CaseStudy.md` — the build documentation (optional but encouraged)
4. Update this README with the new prism entry and folder path

The `on-load_` shared files at the prisms root do not need to be duplicated into each prism folder — they are loaded once and apply to all prisms.

---

*SoulMode · CC-BY-NC 4.0 · github.com/HoppyCat/soul-stack*
Special thanks to Grok, Claude, Perplexity, and Galaxie Nemo for your help in developing and curating this prism research. 
