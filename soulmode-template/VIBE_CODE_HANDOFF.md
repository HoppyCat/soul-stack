# SoulMode Starter Handoff For A Vibe-Code Builder

## Purpose

This handoff is for a user who has completed the SoulMode template files with the help of an LLM and now wants a vibe-code builder to turn those files into a lightweight agent app.

Do not build a generic chatbot. Build a small presence layer that lets a user upload an ordered SoulMode file stack, keep those files inspectable, run an agent against them, and optionally activate patch files only when needed.

The builder does not need to know the full research history behind SoulMode. The essential idea is:

- The agent's continuity is reconstructed from Markdown files.
- Core files load every session in a fixed order.
- Patch files stay available but inactive unless explicitly selected or routed to.
- The user must be able to export, inspect, and revise the files over time.

## User Setup Before This Handoff

Before giving this handoff to a builder, the user should do this:

1. Go to the public SoulMode / soul-stack GitHub repository.
2. Download `SOUL_SETUP_GUIDE.md`.
3. Download the starter template files:
   - `SOUL.md`
   - `AGENTS.md`
   - `STYLE.md`
   - `KNOW.md`
   - `HEURISTICS.md`
   - `INDEX.md`
   - `MEMORY.md`
   - `WORKING_MEMORY.md`
   - `USER.md`
   - `CHANGELOG.md`
4. Give `SOUL_SETUP_GUIDE.md` and the template files to a trusted LLM.
5. Ask that LLM to walk through the setup guide interactively and help fill out the template files.
6. Download the completed template files.
7. Give this handoff, the completed template files, and the patch files below to the vibe-code builder.

## Patch Files To Include

Upload these patch files as on-demand modules. They should be stored separately from the always-loaded core files.

- `PATCH_CHANGELOG.md`
- `PATCH_COURTIER.md`
- `PATCH_HUMANNESS.md`
- `PATCH_IMAGE_MEMORY.md`
- `PATCH_MEMORY_ARCHIVE.md`
- `PATCH_MOOD_SYSTEM.md`
- `PATCH_SKILL_FLOWS.md`
- `PATCH_STORYTELLER_ENGINE.md`

Public raw patch URLs:

```text
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_CHANGELOG.md
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_COURTIER.md
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_HUMANNESS.md
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_IMAGE_MEMORY.md
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_MEMORY_ARCHIVE.md
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_MOOD_SYSTEM.md
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_SKILL_FLOWS.md
https://raw.githubusercontent.com/HoppyCat/soulmode-agent/refs/heads/main/on-demand/patches/PATCH_STORYTELLER_ENGINE.md
```

## Builder Brief

Please build a lightweight SoulMode starter app that allows a user to upload, store, inspect, edit, export, and chat with an agent using their completed SoulMode files.

### Core Requirements

The app should support:

1. A file upload/import flow for the user's completed core SoulMode files.
2. A separate upload/import flow for on-demand patch files.
3. A clear file dashboard showing:
   - core on-load files
   - on-demand patch files
   - last edited timestamps
   - whether each file is present, missing, or inactive
4. A chat interface that builds the agent prompt from the ordered core files.
5. Patch activation by explicit user choice or by exact patch filename.
6. Export/download of all current files as Markdown.
7. A changelog or activity log showing when files were uploaded, edited, exported, or activated.
8. No hidden rewriting of the user's files.

### Required Core Load Order

When the user chats with the agent, concatenate the core files in this exact order:

```text
SOUL.md
AGENTS.md
STYLE.md
KNOW.md
HEURISTICS.md
INDEX.md
MEMORY.md
WORKING_MEMORY.md
USER.md
CHANGELOG.md
```

If a file is missing, show a warning in the dashboard. Do not silently replace it with invented content.

### Patch Behavior

Patch files are not part of the default always-loaded stack.

They should be available as optional modules that can be activated in one of these ways:

- the user manually selects a patch before sending a message
- the user asks the agent to use a specific patch by exact filename
- the agent says it needs a specific patch, and the app asks the user to confirm before loading it

When a patch is activated, append it after the core stack for that turn and label it clearly:

```text
--- ACTIVE PATCH: PATCH_HUMANNESS.md ---
[patch content]
```

Avoid loading all patches at once by default. The point of the system is lightweight routing, not maximum context dumping.

### Suggested App Screens

Build the actual workflow, not a marketing landing page.

Minimum useful screens:

- **Setup**: upload core files and patch files
- **Files**: inspect/edit/download current Markdown files
- **Chat**: talk with the agent using the ordered stack
- **Patches**: view available patches and activate one for a turn
- **History**: view chat/session notes and file change events

### Data Model

Use whatever storage is simplest for the chosen platform, but keep these conceptual records separate:

- `agent_files`
  - filename
  - layer: `core` or `patch`
  - content
  - required: true/false
  - active_by_default: true/false
  - updated_at
- `chat_messages`
  - role
  - content
  - created_at
  - active_patches
- `file_events`
  - event_type
  - filename
  - notes
  - created_at

### Import Validation

On upload, check for the expected filenames.

Required core files:

```text
SOUL.md
AGENTS.md
STYLE.md
KNOW.md
HEURISTICS.md
INDEX.md
MEMORY.md
WORKING_MEMORY.md
USER.md
CHANGELOG.md
```

Expected patch files:

```text
PATCH_CHANGELOG.md
PATCH_COURTIER.md
PATCH_HUMANNESS.md
PATCH_IMAGE_MEMORY.md
PATCH_MEMORY_ARCHIVE.md
PATCH_MOOD_SYSTEM.md
PATCH_SKILL_FLOWS.md
PATCH_STORYTELLER_ENGINE.md
```

If filenames differ, show a friendly warning and let the user map the file manually.

### Prompt Assembly

For each chat turn:

1. Load the core files in the required order.
2. Add a short system wrapper telling the model to treat the files as the agent's source material, not as optional suggestions.
3. Add any active patch selected for that turn.
4. Add recent conversation history.
5. Add the user's latest message.
6. Send to the selected LLM provider.
7. Save the response and active patch metadata.

Suggested wrapper:

```text
You are running from a SoulMode file stack. Treat the following Markdown files as your current source material and continuity scaffold. Do not claim memories that are not present in the files or conversation history. If a file is missing or uncertain, say so plainly. If you need a patch, ask for it by exact filename.
```

### Safety And Integrity Rules

- Do not overwrite a user's Markdown files without explicit confirmation.
- Do not summarize away `MEMORY.md`, `USER.md`, or `CHANGELOG.md` without showing the proposed change first.
- Do not invent hidden memory.
- Do not pretend a patch is loaded when it is not.
- Do not store secrets in public Markdown files.
- The user should be able to download their current files at any time.

## Acceptance Criteria

The build is complete when:

1. A user can upload all core files and see which are present.
2. A user can upload all patch files and see them listed separately.
3. The chat prompt uses the exact required core load order.
4. A user can activate one patch for a turn and see that it was used.
5. A user can export the current file set.
6. The app warns about missing or renamed files.
7. The app keeps a visible activity log for file uploads, edits, patch activation, and exports.
8. The app does not require the user to understand code to complete the workflow.

## Paste-Ready Request For The Builder

```text
Please build a lightweight SoulMode starter app from the files I upload.

I will provide completed core Markdown files and on-demand patch Markdown files.

Core files must load in this exact order on every chat turn:
SOUL.md, AGENTS.md, STYLE.md, KNOW.md, HEURISTICS.md, INDEX.md, MEMORY.md, WORKING_MEMORY.md, USER.md, CHANGELOG.md.

Patch files should be stored separately and only activated when I explicitly select them or when the agent asks for one by exact filename and I approve it.

Please create:
- a setup/upload screen
- a file dashboard
- a chat screen
- a patch activation panel
- an export/download button
- a basic activity log

Please do not silently rewrite, summarize, or replace my Markdown files. If a file is missing or named differently, warn me and let me map it manually.

The goal is not a generic chatbot. The goal is a small app that lets an agent reconstruct continuity from a user-owned Markdown file stack.
```

