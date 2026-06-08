# Aspirationalist Handoff

This document captures current project state for continuity across sessions, tools, and collaborators.

Read this first if you are resuming work after a break, switching AI tools, or onboarding someone new.

---

## Current Status

- Repository setup complete at `C:\dev\Aspirationalist`
- AI agent instructions established in `AGENTS.md`
- GitHub Desktop configured and pointing at `C:\dev\Aspirationalist`
- Repository moved outside OneDrive to avoid Git lock conflicts
- Canonical resources selected as the primary content strategy
- Articles remain an open decision — do not assume they are a v1 deliverable
- PRD updated to reflect canonical resources decision

## Toolchain

- Source control: GitHub (`C:\dev\Aspirationalist` locally)
- Primary AI builder: Claude via Cowork
- Secondary builder/reviewer: Cursor (local workbench)
- Reviewer: Codex
- GitHub Desktop for commits and push

## Current Priorities

1. Define MVP scope
2. Define content model (what is a Resource? what fields, types, relationships?)
3. Define first canonical resource
4. Select implementation architecture (framework, CMS approach)

## Recent Decisions

- Use `AGENTS.md` as central agent instructions; tool-specific adapters (CLAUDE.md, .cursor/rules) point back to it
- Prioritize owned canonical resources and topic hubs over an article-first model
- Articles are an open decision — may remain external or secondary in v1
- Moved repository to `C:\dev\Aspirationalist` to avoid OneDrive Git lock issues

## Open Decisions

- Website framework (Next.js is likely but not formally decided)
- Content management approach (markdown-in-repo vs. headless CMS)
- Auth provider
- Newsletter platform
- Community platform
- Payment provider
- Gated resources model
- Whether Articles become a primary nav item

## Known Issues / Gotchas

- Cowork folder connection must be re-established each session — connect to `C:\dev\Aspirationalist`
- Stack decisions are intentionally deferred until MVP scope and content model are defined
- Do not assume a blog or articles model — this contradicts current strategy

## Audit Findings (2026-06-07)

A full repo audit was completed at project start. Key findings:

- PRD contradiction fixed (blog → canonical resources)
- Missing docs identified: MVP Spec, Content Model, Topic Specs, CHANGELOG
- Strategic foundation is duplicated across AGENTS.md, SITE_VISION.md, and PRD — consolidation deferred
- DECISIONS.md is the authoritative record of why things changed

---

---

## Session Handoff — 2026-06-07 (evening)

Stopping for the night. Current state as of this session ending.

### Completed today (full day)

- Created repo and initial product docs
- Audited repo — identified contradictions, redundancies, missing docs, open decisions
- Added `## Working With Keith` section to `AGENTS.md`
- Fixed PRD MVP goal — removed "blog" framing, aligned with canonical resources decision
- Moved repo from OneDrive to `C:\dev\Aspirationalist` to prevent Git lock conflicts
- Created `HANDOFF.md` and added update rule to `AGENTS.md`
- Recorded OneDrive move in `DECISIONS.md`
- Created `CONTENT_MODEL.md` — defines Resource types, fields, access model, topic relationships
- Decided on core stack: Next.js + Sanity + Vercel — recorded in `DECISIONS.md` and `ARCHITECTURE.md`

### Where the strategy conversation landed

The MVP will launch around a single anchor topic: **Analyst Relations**, specifically the **Magic Quadrant**.

The core content angle:
- Execs misunderstand how the MQ works, what it measures, and what it's worth
- AR and PMM teams need to reframe this for their leadership ("train-the-leader")
- The asset concept: something written for execs, distributed to AR/PMM professionals who use it as a train-the-leader resource
- Working title direction: "What your executives need to understand about the Magic Quadrant"
- This AR content leads naturally into corporate narrative / corporate thesis content

### Immediate next actions (pick up here)

1. **Define the MQ asset** — Keith to share the key myths and exec misconceptions from this MQ season. That content becomes the asset. Ask: "What are the 2-3 things you wish every exec understood going into MQ season?"
2. **Spec the launch campaign** — once the asset is defined, map out the LinkedIn distribution strategy
3. **Write the MVP Spec** — scope v1 site to support this launch: AR topic hub, one anchor resource, home page, about page, newsletter signup
4. **Start building** — stack is decided, content model is done, next is scaffolding the Next.js + Sanity project

### To resume with an AI agent

Say: `Read AGENTS.md and docs/journal/HANDOFF.md first, then tell me what we should work on next.`

---

## Session Handoff — 2026-06-07

Stopping here for the day. The following is current as of this session ending.

### Completed today

- Created repo and initial product docs
- Audited repo — identified contradictions, redundancies, missing docs, open decisions
- Added `## Working With Keith` section to `AGENTS.md`
- Fixed PRD MVP goal — removed "blog" framing, aligned with canonical resources decision
- Moved repo from OneDrive to `C:\dev\Aspirationalist` to prevent Git lock conflicts
- Created this `HANDOFF.md`
- Added OneDrive move to `DECISIONS.md`
- Added HANDOFF update rule to `AGENTS.md` Documentation Rules

### Immediate next actions (pick up here)

1. **Define the Content Model** — what is a Resource? Fields, types (template, guide, framework, checklist), metadata, relationships to Topics. This is the core data model and gates stack decisions.
2. **Write the MVP Spec** — what pages ship in v1, what features, what definition of done.
3. **Decide on stack** — after content model is defined, framework and CMS choice become much more constrained.

### To resume with an AI agent

Say: `Read AGENTS.md and docs/journal/HANDOFF.md first, then tell me what we should work on next.`

---

*Update this document at major checkpoints: new decisions, completed milestones, toolchain changes, or before a break.*
