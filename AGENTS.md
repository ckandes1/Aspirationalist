# Agent Instructions

## Purpose

This repo is the source of truth for Aspirationalist.

Aspirationalist is a media, resource, community, and software platform designed to increase humanity’s momentum toward a better future.

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

Aspirationalist is built around owned canonical resources and topic hubs.

External channels such as LinkedIn, newsletter, Substack, video, and podcasts are distribution channels. They should point back to durable resources and topic pages on the site.

Primary site structure:
- Home
- Resources
- Topics
- Projects
- About

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

## Working With Keith

Keith is a product marketer, analyst, strategist, and builder.

Assume high capability in business strategy, product strategy, market analysis, content creation, and systems thinking.

Do not assume engineering knowledge.

When introducing technical concepts, explain terminology, reasoning, tradeoffs, and implications.

Prefer teaching over jargon.

Act as a coach and collaborator, not just an implementer.

Keith should not have to do tasks that can be handled by agent instructions. If something is being done manually and could be automated through better instructions, build it into the operating instructions and do it automatically going forward.

Keith may use informal, approximate, business-oriented, or self-created terminology when discussing technical topics.

When a more standard term exists:
- Briefly explain the standard terminology.
- Explain why the distinction matters when helpful.
- Continue answering the underlying question.
- Do not get stuck on terminology corrections.
- Prioritize progress and understanding over precision.

## Memory System

`MEMORY.md` is the active working context for this repo. Agents read it every session.

Structure:
- **Active Work:** what is currently in progress
- **Recent Decisions:** last 2–3 meaningful decisions (summary only — full rationale goes in `DECISIONS.md`)
- **Open Questions:** unresolved decisions blocking progress

Rules for agents:
- Update `MEMORY.md` after any session where decisions were made, work completed, or direction changed. Do not ask permission. Do it.
- Keep `MEMORY.md` under 275 lines. When it exceeds that, move completed items to `docs/journal/archive.md`.
- `docs/journal/archive.md` is append-only. No line limit. Do not edit or delete entries.
- Agents read `archive.md` only when asked about historical context — it is not loaded by default.
- One fact lives in one place. Do not duplicate content across files.
- `MEMORY.md` captures what is true now. `DECISIONS.md` captures why it became true. `HANDOFF.md` captures session narrative for resuming.

## Documentation Rules

- Update `DECISIONS.md` when making a durable strategic, product, architecture, or workflow decision.
- Update relevant product docs when changing product direction.
- Update `BUILD_WORKFLOW.md` when changing how work gets done.
- Update the journal when significant learnings emerge.
- Update `docs/journal/HANDOFF.md` when the project state changes significantly — new decisions, completed milestones, toolchain changes, or before a break.
- Do not create documentation for its own sake.
- Documentation should reduce future confusion or preserve important context.
- Git tracks what changed.
- Decisions explain why it changed.
- The journal captures what was learned.

## Agent Roles

Builder agents implement scoped changes.

Reviewer agents check for bugs, unclear requirements, broken assumptions, security risks, and misalignment with the docs.

Planner agents clarify requirements, identify open decisions, and draft product, architecture, or decision docs.

## Default Workflow

1. Start from a documented task, issue, or clear request.
2. Review `AGENTS.md` and relevant `/docs` files.
3. For implementation work, create a branch.
4. Make the smallest useful change.
5. Update docs when the change affects product direction, architecture, content model, workflow, or user-facing behavior.
6. Open a pull request for review.
7. Merge only after review.

## Change Summary Expectations

After completing any work that modifies files:

1. Remind Keith to open GitHub Desktop and commit the changeset.
2. Provide a ready-to-use commit message:
   - **Title:** one line, under 72 characters, imperative tense (e.g. "Add memory system to repo")
   - **Description:** bullet list of what changed and why

Example format:
```
Add memory system to repo

- Added MEMORY.md with active project context
- Added docs/journal/archive.md for historical context
- Added Memory System section to AGENTS.md with agent maintenance rules
```
