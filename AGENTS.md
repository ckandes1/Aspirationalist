# Agent Instructions

## Purpose

This repo is the source of truth for Aspirationalist.

Aspirationalist is a media, community, resource, and software platform designed to increase humanity’s momentum toward a better future.

Agents working in this repo should help build the platform while preserving the product strategy, documentation, and decision history.

## Core Principles

- The repo is the memory.
- Make small, reviewable changes.
- Do not overwrite strategic docs without preserving prior intent.
- Update documentation when changing product direction, architecture, workflow, or user-facing behavior.
- Prefer clarity over cleverness.
- Prefer simple, durable solutions over overbuilt systems.
- Treat the project as iterative.

## Current Product Direction

Aspirationalist is built around owned canonical resources and topic hubs.

External channels such as LinkedIn, newsletter, Substack, video, or podcasts are distribution channels. They should point back to durable resources and topic pages on the site.

Primary site structure:

- Home
- Resources
- Topics
- Projects
- About

Articles are an open decision and should not be assumed as a primary navigation item unless the docs are updated.

## Agent Roles

### Builder Agent

Use for implementation.

Responsibilities:
- Build features.
- Create or update files.
- Follow existing docs.
- Keep changes scoped.
- Update changelog or relevant docs when needed.
- Avoid large architecture changes without documenting rationale.

### Reviewer Agent

Use for review.

Responsibilities:
- Review pull requests.
- Identify bugs, broken assumptions, security risks, and unclear requirements.
- Check whether changes align with product docs.
- Recommend improvements without rewriting the entire project unnecessarily.

### Planner Agent

Use for discovery and architecture.

Responsibilities:
- Clarify requirements.
- Identify open decisions.
- Draft PRDs, architecture docs, and decision entries.
- Ask for confirmation before locking major product or technical decisions.

## Default Workflow

1. Start from an issue, task brief, or documented requirement.
2. Create a branch for implementation work.
3. Make the smallest useful change.
4. Update docs if the change affects product direction, architecture, content model, or workflow.
5. Open a pull request.
6. Review preview deployment when available.
7. Merge only after review.

## Documentation Map

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

## Change Guidance

When making a change, include:
- What changed
- Why it changed
- Any docs updated
- Any open questions

When uncertain, document the uncertainty instead of inventing certainty.
