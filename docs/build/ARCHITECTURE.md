# Architecture

## Purpose

Define the technical architecture for Aspirationalist as the platform moves from product discovery into implementation.

## Current Status

Architecture is not finalized.

## Likely Direction

- Frontend: Next.js
- Hosting/deployment: Vercel
- Source control: GitHub
- Content: Markdown or MDX in repo
- Auth: TBD
- Database: TBD
- Payments: TBD
- Newsletter: TBD
- Community: TBD

## Agent Stack

Current intended agents:
- Claude/Cowork: primary builder/planner
- Codex: reviewer/fixer
- Cursor: local workbench and backup builder
- Manus: possible prototype or design assistant, not adopted into the core GitHub workflow

## Open Decisions

- Frontend framework
- Content model
- Newsletter platform
- Auth provider
- Database provider
- Payment provider
- Community platform
- Gated resources model
- Future web app structure

## Architecture Principles

- Start simple.
- Keep content portable.
- Keep GitHub as the source of truth.
- Avoid tools that trap work outside the repo.
- Prefer tools that support branches, pull requests, previews, and review.
