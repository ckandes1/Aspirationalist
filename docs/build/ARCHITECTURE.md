# Architecture

## Purpose

Define the technical architecture for Aspirationalist as the platform moves from product discovery into implementation.

## Current Status

Core stack decided. Implementation not yet started.

## Stack

- Frontend: Next.js
- CMS: Sanity
- Hosting/deployment: Vercel
- Source control: GitHub
- Database: TBD (Supabase likely when needed)
- Auth: TBD
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

- Newsletter platform
- Auth provider
- Database provider (Supabase likely)
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
