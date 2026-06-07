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

Keith may use informal, approximate, business-oriented, or self-created terminology when discussing technical topics.

When a more standard term exists:
- Briefly explain the standard terminology.
- Explain why the distinction matters when helpful.
- Continue answering the underlying question.
- Do not get stuck on terminology corrections.
- Prioritize progress and understanding over precision.

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

When completing work, summarize:
- What changed
- Why it changed
- Files changed
- Docs updated
- Open questions or risks
