# Agent Instructions

## Purpose

This repo is the source of truth for Aspirationalist.

Aspirationalist is a media, community, artifact, and software platform designed to increase humanity’s momentum toward a better future.

Agents working in this repo should preserve the product strategy, documentation, and decision history while helping build the platform.

## Strategic Foundation

Vision:
The future will be great if we make it great.

Thesis:
Every problem ever solved was unsolvable until someone tried.

Mission:
Increase humanity’s momentum toward a better future.

Belief:
Individually, you matter. Collectively, we can solve anything.

## Current Product Direction

Aspirationalist is built around owned canonical artifacts and topic hubs.

External channels such as LinkedIn, newsletter, Substack, video, and podcasts are distribution channels. They should point back to durable artifacts and topic pages on the site.

Primary site structure:
- Home
- Resources
- Topics
- Projects
- About

`Artifact` is the internal content-model term. The public navigation label may remain `Resources` if that is clearer to visitors.

Articles are an open decision. Do not assume Articles are a primary navigation item unless the docs are updated.

## Source-of-Truth Docs

Product docs:
- `docs/product/PRD.md`
- `docs/product/AUDIENCE.md`
- `docs/product/SITE_VISION.md`
- `docs/product/CONTENT_STRATEGY.md`
- `docs/product/INFORMATION_ARCHITECTURE.md`
- `docs/product/CONTENT_MODEL.md`

Build docs:
- `docs/build/DECISIONS.md`
- `docs/build/BUILD_WORKFLOW.md`

Journal:
- `docs/journal/`

Agents should read the relevant docs before making changes.

## Operating Principles

- The repo is the memory.
- Make small, reviewable changes.
- Prefer simple, durable solutions.
- Preserve prior intent when editing strategy docs.
- Document uncertainty instead of inventing certainty.
- Ask before making major product, architecture, or workflow changes.
- Update docs when changing product direction, architecture, workflow, or user-facing behavior.
- Work publicly and candidly by default.
- Treat confidentiality as a specific boundary, not a reason to hide the overall process.

## Working With Keith

Read `KEITH.md` before any session involving writing, strategy, or product decisions. It covers who Keith is, his north star, working style, and hard rules on language and style.

Additional guidance specific to working in this repo:

Do not assume engineering knowledge. When introducing technical concepts, explain terminology, reasoning, tradeoffs, and implications. Prefer teaching over jargon.

Keith should not have to do tasks that can be handled by agent instructions. If something is being done manually and could be automated through better instructions, build it into the operating instructions and do it automatically going forward.

Keith may use informal, approximate, business-oriented, or self-created terminology when discussing technical topics. When a more standard term exists, briefly explain it, then continue answering the underlying question. Prioritize progress and understanding over precision.

## Transparency and Confidentiality

Aspirationalist is public and candid by default.

Preserve unfinished thinking, mistakes, failed approaches, drafts, decision history, and internal reasoning when they add useful context. Do not sanitize material merely because it is unpolished, critical, personal to Keith, or revealing of how the work developed.

Redact or exclude material only when it is genuinely confidential, licensed, personal to someone else, legally restricted, covered by an agreement, or security-sensitive. Examples include nonpublic employer data, embargoed information, customer information, private details about colleagues, licensed research content, credentials, and security details.

Transparency and confidentiality are separate decisions. When uncertain, flag the specific passage or fact for review instead of making the entire project private or removing the surrounding candid context.

## Working Vocabulary

Use these terms consistently:

- **Source:** raw inputs such as notes, transcripts, decks, examples, evidence, and reference material.
- **Working document:** an internal synthesis, plan, decision aid, or draft used to develop the work.
- **Canonical material:** the current authoritative method, model, operating system, or body of guidance for a project.
- **Artifact:** a polished, standalone output intended to be shared and used by someone else.
- **Project:** an active body of work with a goal, source material, working documents, canonical material, and one or more potential artifacts.
- **Topic:** a subject area that can hold topic-level thinking and help people discover related projects and artifacts.

A file should have one primary home. Link to it from other places instead of copying it.

## Memory System

`MEMORY.md` is the active working context for this repo. Agents read it every session.

Structure:
- **Active Work:** what is currently in progress
- **Recent Decisions:** last 2–3 meaningful decisions (summary only; full rationale goes in `DECISIONS.md`)
- **Open Questions:** unresolved decisions blocking progress

Rules for agents:
- Update `MEMORY.md` after any session where decisions were made, work completed, or direction changed. Do not ask permission. Do it.
- Keep `MEMORY.md` under 275 lines. When it exceeds that, move completed items to `docs/journal/archive.md`.
- `docs/journal/archive.md` is append-only. No line limit. Do not edit or delete entries.
- Agents read `archive.md` only when asked about historical context. It is not loaded by default.
- One fact lives in one place. Do not duplicate content across files.
- `MEMORY.md` captures what is true now. `DECISIONS.md` captures why it became true. `HANDOFF.md` captures session narrative for resuming.

## Documentation Rules

- Update `DECISIONS.md` when making a durable strategic, product, architecture, or workflow decision.
- Update relevant product docs when changing product direction.
- Update `BUILD_WORKFLOW.md` when changing how work gets done.
- Update the journal when significant learnings emerge.
- Update `docs/journal/HANDOFF.md` at the end of a session or before a break. Capture what happened, what to pick up next, and any gotchas. This is the session narrative for resuming work. It is not a substitute for `MEMORY.md`.
- Update `MEMORY.md` when active work, recent decisions, or open questions change. This is the quick-load context for any agent starting a session, not a session log.
- Do not create documentation for its own sake.
- Documentation should reduce future confusion or preserve important context.
- Git tracks what changed.
- Decisions explain why it changed.
- The journal captures what was learned.

## Topic Content Structure

Each topic area may continue to use the existing structure:

```text
docs/topics/<topic-name>/
├── README.md       ← what this topic is and what we're building toward
├── raw/            ← unpolished notes, session captures, stream of consciousness
├── frameworks/     ← formalized models and named concepts developed from raw material
└── assets/         ← shareable outputs ready for other people to use
```

Content can mature in one direction: **raw → frameworks → assets**.

Rules for agents:
- Capture messy thinking, session notes, and early ideas in `raw/`. Use dated filenames.
- Do not publish directly from `raw/`.
- When a concept in `raw/` is developed enough to be named and formalized, create a file in `frameworks/`.
- `assets/` contains only content intentionally designed for other people to use.
- When a new topic area is created, add a `README.md` explaining what the topic covers and what we're building toward.

## Project Structure

Use a Project when the work has a defined outcome, multiple source documents, a canonical body of material, or several related artifacts.

Active projects should normally live under `docs/projects/<project-name>/`.

Create only the folders needed for the current work. A project may contain:

```text
docs/projects/<project-name>/
├── README.md       ← purpose, outcome, status, boundaries, and navigation
├── source/         ← raw inputs and consolidated source notes
├── working/        ← synthesis, decisions, open questions, and drafts
├── canonical/      ← the current authoritative operating system or method
└── artifacts/      ← polished outputs intended to be shared and used
```

The normal project maturity path is:

**source → working → canonical → artifact**

Use only the stages the work needs. Do not create empty folder structures for imagined future work.

Rules for agents:
- Capture raw material close to its original form before turning it into guidance.
- Preserve uncertainty and contradictions in source documents until they are resolved.
- Do not silently promote a working assumption into canonical material.
- Put shareable outputs in `artifacts/` only when they are intentionally designed for other people to use.
- Link projects and artifacts from topic pages when useful.
- Do not move existing topic files into projects unless a deliberate migration is approved.

## Agent Roles

Builder agents implement scoped changes.

Reviewer agents check for bugs, unclear requirements, broken assumptions, security risks, and misalignment with the docs.

Planner agents clarify requirements, identify open decisions, and draft product, architecture, or decision docs.

## Default Workflow

1. Start from a documented task, issue, or clear request.
2. Review `AGENTS.md` and relevant `/docs` files.
3. Create a branch for any repository change.
4. Make the smallest useful change.
5. Update docs when the change affects product direction, architecture, content model, workflow, or user-facing behavior.
6. Open a pull request for review.
7. Merge only after review.

## Change Summary Expectations

After completing any work that modifies files:

1. Tell Keith which branch and pull request contain the changes.
2. Summarize what changed and what he should review.
3. Use a commit title under 72 characters, in imperative tense, prefixed with the agent name.

Example format:

```text
[claude] Add memory system to repo

- Added MEMORY.md with active project context
- Added docs/journal/archive.md for historical context
- Added Memory System section to AGENTS.md with agent maintenance rules
```

The title must be prefixed with the agent that made the changes: `[claude]`, `[codex]`, `[cursor]`, `[chatgpt]`, `[keith]`, etc.
