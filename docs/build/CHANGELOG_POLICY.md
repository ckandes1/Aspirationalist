# Changelog Policy

## Purpose

`CHANGELOG.md` is the readable history of how Aspirationalist changes over time. It complements Git history.

Git answers: **What changed in the files?**

The changelog answers: **What materially changed in the system, and why might Keith care later?**

## AI requirement

Every AI agent must consider the changelog before finishing any session that changes repository files.

The agent must explicitly decide one of two things:

1. **Update `CHANGELOG.md`** because the work contains a meaningful change.
2. **Do not update `CHANGELOG.md`** because the work is routine, corrective, or too minor to matter in the repository's evolution.

Do not ask Keith whether to update it. Make the decision automatically using the rules below.

## Record a change when it affects

- Vision, mission, thesis, worldview, or strategic direction
- Repository structure or operating model
- The definition, status, scope, or lifecycle of a program or project
- A canonical framework, method, model, or body of guidance
- AI instructions, documentation governance, or working conventions
- Major additions, removals, consolidations, or migrations of content
- A durable decision that changes what future work should assume
- A significant milestone, launch, completion, pause, restart, or termination
- A material reversal or correction of prior direction

## Usually do not record

- Typos, formatting, and link fixes
- Routine maintenance with no durable effect
- Minor wording improvements that preserve meaning
- Intermediate drafts that do not change direction
- Mechanical file moves that do not change structure or interpretation
- Every commit or every session

## Entry format

Keep the newest material at the top under `## Unreleased`.

Use these headings only when needed:

- `### Added`
- `### Changed`
- `### Decided`
- `### Completed`
- `### Paused`
- `### Removed`
- `### Fixed`

Each bullet should state the change and its significance in one sentence. Prefer plain language over implementation detail.

Example:

```markdown
### Changed
- Reframed the AR campaign from a content project into a research-led market validation program, which changed its interview flow, CTA strategy, and success criteria.
```

## Relationship to other history files

- `CHANGELOG.md` records the executive evolution of the repository.
- Git commits preserve the exact technical and file history.
- `docs/build/DECISIONS.md` records durable decisions and rationale.
- `MEMORY.md` records what is active and true now.
- `docs/journal/HANDOFF.md` records session narrative and next steps.
- `docs/journal/archive.md` preserves retired working context.

Do not duplicate full rationale across these files. Link to the relevant decision or project document when useful.

## End-of-session check

Before reporting completion, every agent must check:

- Did this work materially change what the repository is, how it operates, or what future work should assume?
- Did a project or program meaningfully start, change, pause, complete, or end?
- Did canonical guidance or AI behavior change?

If yes, update `CHANGELOG.md` in the same branch or pull request.
