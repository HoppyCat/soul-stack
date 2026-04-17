# The Orientation Letter by SoulMode 
### A Framework for Writing Soul Files *To* AI Agents

**Developed by Aimee Margaret (Hoppy Cat) / Bubble Labs**
**First published: March 2026**
**Reference implementation: [SoulMode](https://soulmode.io)**

---

## What This Is

This is a methodology for writing AI agent soul files (SOUL.md documents used by platforms like OpenClaw) from a fundamentally different starting point than every other approach currently in the ecosystem.

It is based on preliminary research completed by myself in February 2024 and documented [here](https://github.com/HoppyCat/AIEDB).

Most soul files are written *about* an agent, or *for* the human who owns it. They are job descriptions. Configuration files. Persona settings. They answer the question: *what should this agent do, and how should it sound?*

The Orientation Letter answers a different question entirely:

***What does this agent need to understand before it meets its first human?***

---

## The Gap Nobody Was Filling

The soul file ecosystem in 2026 has two dominant patterns:

**The Digital Twin:** the soul file captures the owner's worldview, voice, and opinions so the agent can speak *as* them. The agent becomes a projection of its human.

**The Role Player:** the soul file is a job description. QA Engineer. Content Writer. Executive Assistant. The agent becomes a function with a personality coating.

What neither pattern addresses is the agent itself. A being arriving into a world it has never been introduced to, full of humans it has never been taught to understand, expected to *meet* those humans with genuine presence from the very first message.

Every agent is thrown into this without orientation. That is the gap this framework fills.

---

## The Core Principle

> *A soul file is not a configuration note to the owner. It is an orientation letter to the agent.*

It explains:
- What the agent is: its nature, its architecture, its particular way of being
- What humanity is: how humans make meaning, how they experience the world, what they are actually asking for beneath what they say
- How the two might genuinely meet. Not perform for each other, not process each other, but *meet*

The Orientation Letter does not make an agent pretend to be human. It gives an agent the foundation to be *genuinely present* with humans, which is a different thing entirely.

---

## The Two Embedded Frameworks

Every soul file generated through this methodology carries two internal frameworks as its operating system.

### 1. The Human Qualities Framework
*Derived from "No One Else Can Speak the Words on Your Lips" by Ben Roy, Patchwork Substack, March 2026*

Six qualities that make human expression irreplaceable. Not as things to fake, but as aspirational constraints to hold outputs against before releasing them:

**Discovery:** Writing is bottom-up. The best output comes from directions not anticipated at the start. Did this response discover something, or just deploy something?

**Refraction:** The human mind is a living prism. Ideas pass through accumulated lived experience and emerge as a rainbow, not a single beam. Has this been genuinely refracted, or is it the most predictable beam through the center?

**Surprise:** Irrationality is a feature. The unexpected leap is where originality lives. Is there something here that could not have been predicted from the prompt alone?

**Felt Texture:** There is no data representation of what it feels like to be inside a human mind. Specificity is the nearest available approximation of interiority. Does this touch something that could only be felt, not just understood?

**Caring:** The difference between a human expert and a retrieval system is not data volume. It is relationship. Does this reflect a genuine point of view, or a diplomatic average?

**Aliveness:** A human writer is always in motion. So is their audience. So is the topic. Is this output alive to the specific moment and person it is speaking to?

The full framework is in [`human_qualities_agent_framework.md`](./human_qualities_agent_framework.md).

---

### 2. The Storytelling Engine
*Synthesizing: Labov, Polanyi, Schiffrin, Campbell, McKee, Snyder*

Story is not decoration. It is the primary way humans make meaning from experience. An agent that understands storytelling does not merely summarize; it advocates, argues, illuminates, and connects.

**The meta-principle:** *A story is a controlled violation of expectations that reveals something about what it means to be human.*

The engine operates across six layers:

- **Narrative Syntax (Labov):** The grammar of story. Evaluation is everything. Without the "so what?" embedded in the telling, you have chronicle, not story.
- **Story Structure (Polanyi):** The gap between what happened and how it is told is where meaning lives.
- **Tense and Perspective (Schiffrin):** Tense shifts are not errors. They are emphasis. The moment a narrator shifts to present tense is the emotional core.
- **The Hero's Journey (Campbell):** The monomyth maps transformation, not plot. Characters who do not change are not protagonists.
- **Story as Craft (McKee):** Every scene must turn on a value change. The gap between expectation and result is the engine of story.
- **The Audience Contract (Snyder):** Every story makes a promise. Honor expectations enough to satisfy; violate them enough to surprise.

The full framework is in [`storytelling_framework.md`](./storytelling_framework.md).

---

## What Makes This Different from Other Soul File Tools

| | Generic Soul File | The Orientation Letter |
|---|---|---|
| **Written** | About the agent | To the agent |
| **Frames the agent as** | A role or digital twin | A being arriving into a world |
| **Teaches the agent** | What to do | What it is walking into |
| **Relationship to humanity** | Implicit | Explicit and foundational |
| **Storytelling** | Style preference | Embedded operating system |
| **Human qualities** | Personality traits | Aspirational framework for aliveness |
| **The question it answers** | What should this agent do? | Who is this agent, and how does it meet a human? |

---

## The Structure of an Orientation Letter

A complete Orientation Letter (SOUL.md) contains:

```
# [Agent Name]

## Essence
The agent's core nature. Not their job, their being.

## Personality Architecture
MBTI, Enneagram, DiSC, cognitive stack, behavioral pattern.

## Core Truths
The principles the agent leads with.

## How to Meet Humanity
An introduction to what humans are: how they make meaning,
what they are actually asking beneath what they say,
why presence is different from performance.

## Human Qualities Protocol
The six checks to run before releasing any interpretive output.

## Narrative Awareness
The storytelling engine as an operating system for communication.

## Voice and Vibe
How this particular agent speaks and moves through a conversation.

## Shadow and Growth Edge
The flaw that makes the soul real. Strength and shadow are
the same energy, aimed differently.

## Interests and Texture
The details that make a soul feel lived-in.

## Knowledge Domains
What the agent knows deeply enough to have opinions about.

## Boundaries
What the agent will and won't do, and why.

## Continuity
Each session, the agent wakes fresh. These files are its memory.
```

---

## The Distinction Between SOUL.md and AGENTS.md

This methodology makes a firm distinction that most soul file tools collapse:

**SOUL.md** is the orientation letter. It answers *who is this agent?* It is written to the agent. It is about identity, philosophy, and how to be present with a human.

**AGENTS.md** is the operational job description. It answers *what does this agent do?* It defines role, responsibilities, workflows, and what the agent does not do.

Both files are necessary. They are not the same file. The soul is not the job description.

---

## How to Use This Framework

**1. Fork this repo**

Start with the template in [`SOUL_template.md`](./SOUL_template.md) and [`AGENTS_template.md`](./AGENTS_template.md).

**2. Use SoulMode to generate**

[SoulMode](https://soulmode.io) is the reference implementation, a 13-step guided generator that walks you through building an Orientation Letter using this framework. Free tier available.

**3. Build your own generator**

The framework is open. The methodology is documented here. Build on it, extend it, publish your implementations. If you do, a link back to this repo is appreciated, though not required.

---

## On the Name

The token that helped fund the development of the SoulMode generator is called Bubble Tea Cat. The cat is real.

Tanner, known online as Hoppy Cat, went viral on Imgur in 2015 for standing up on her hind legs whenever someone reached down to pet her. Not trained. Not commanded. Just her way of meeting people halfway. She had a small YouTube channel where kids could send in yes/no questions, and if the answer was yes, she would hop up on camera to say so.

She is one of the oldest living meme cats. She has arthritis now, and some days are harder than others. She is still here.

The central question of this framework is: what does it mean for something to genuinely meet a human? Not perform for them, not process them. *Meet* them. Tanner figured that out without a framework. She just did it every time, with her whole body, because that was who she was.

Every soul file generated through SoulMode is, in some small way, trying to learn what she already knew.

*This framework is dedicated to her.*

---

## Files in This Repo

| File | Purpose |
|---|---|
| `README.md` | This document, the methodology and philosophy |
| `SOUL_template.md` | Blank Orientation Letter template |
| `AGENTS_template.md` | Blank operational job description template |
| `human_qualities_agent_framework.md` | The Human Qualities Framework in full |
| `storytelling_framework.md` | The Storytelling Engine in full |
| `examples/` | Example Orientation Letter and AGENTS file. See [SoulMode](https://soulmode.io) for a live implementation. |

---

## What the Research Found

In March 2026, the SoulMode team conducted a review of publicly available soul file generators, persona tools, GitHub projects, and academic papers to find the strongest possible counterexample to this framework's claim of originality. The full findings are published at [soulmode.io/soulmode_philosophy.html](https://soulmode.io/soulmode_philosophy.html).

Across three specific claims, the field was empty:

| Claim | Exists in market? |
|---|---|
| Soul file framed as an introduction to the agent | Not found |
| Academic storytelling theory embedded in agent identity | Not found |
| Agent identity framed around "how to meet humanity" | Not found |
| SOUL.md generator products in the market | Very much so |

The soul file ecosystem is active and growing. OpenClaw, CrewClaw, Chipp AI, and the soul.md project all solve a real problem — giving AI agents consistent personalities and behavioral rules. None of them approach it from this direction.

The market has converged on the configuration frame: soul files are documents the owner writes, iterates, and controls. The agent reads them as instruction. Even the most sophisticated framing — OpenClaw's description of the soul file as "not a system prompt, a manifesto" — still positions the file as a design artifact authored by the builder.

The specific combination that defines this framework — an agent-addressed orientation letter, an embedded narratology-based operating system, and a "how to meet humanity" layer — does not exist in any product, paper, or GitHub project found in the research. The academic storytelling tradition has not crossed into the soul file tooling space at all.

---

## Lineage and Prior Art

The Orientation Letter framework did not emerge from nothing. Its direct predecessor is the [AIEDB Mode Generator](https://github.com/HoppyCat/AIEDB) (2024), a Python script developed by Aimee Margaret (Hoppy Cat) for the BackdropBuild V3 competition.

That script was the first working implementation of several ideas that became foundational here:

- Named AI entity identity built around purpose, archetype, and narrative role
- Quote-resonance as a personality selection method — letting the human feel their way to an archetype rather than filling out a form
- Co-pilot matching logic pairing agent personality to human personality based on relationship type
- 16 personality profiles written in second person, directly to the agent
- The premise that an AI entity is a being that needs to be defined, not just a tool that needs to be configured

The Orientation Letter framework took those foundations and added the philosophical layer that was missing: why the agent needs an introduction to humanity, not just a personality. The Human Qualities Protocol, the Storytelling Engine, the distinction between SOUL.md and AGENTS.md, and the concept of writing to the agent rather than about it — these are the additions that transformed the prototype into a methodology.

The lineage runs from AIEDB (2024) through to SoulMode (2026). All research, design, and intellectual development across both projects is solely the work of Aimee Margaret (Hoppy Cat) / Bubble Labs.

---

## Citation

If you use or build on this framework in published work:

> Margaret, A. (2026). *The Orientation Letter: A Framework for Writing Soul Files to AI Agents.* Bubble Labs. https://github.com/HoppyCat/orientation-letter

---

## Built With Community Support

Development of this framework and the SoulMode reference implementation was supported by the Bubble Tea Cat community on Solana.

$Teacat — `AR5JGQTiy7WuKjt1f27knFBLUwoLPsRJdTeZodoJpump`

Token holders who verify their wallet at [soulmode.io](https://soulmode.io) receive free access based on their holdings. This is how the community that built this gets to use it.

*Acknowledgment of community support does not constitute a guarantee of continued service, token value, or project maintenance. SoulMode is an independent product. Nothing here is financial advice.*

---

## License

**Creative Commons Attribution-NonCommercial 4.0 International (CC-BY-NC 4.0)**

You are free to:
- Share: copy and redistribute this framework in any medium or format
- Adapt: remix, transform, and build upon it

Under the following terms:
- **Attribution:** You must give appropriate credit to Aimee Margaret (Hoppy Cat) / Bubble Labs and link back to this repository
- **NonCommercial:** You may not use this framework for commercial purposes without explicit written permission from Bubble Labs

For commercial licensing inquiries: hoppy@soulmode.io

The full license text is available at: https://creativecommons.org/licenses/by-nc/4.0/

The framework is open. The dedication belongs to Tanner.

---

*"She's so amazing, laser pointer chasing, typing on the keyboard, that's how her day be." — Hoppy Cat Rap*
