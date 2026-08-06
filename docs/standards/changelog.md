# Changelog Standard

## Purpose

`CHANGELOG.md` is the readable executive history of how Aspirationalist changes over time. It complements Git history.

Git answers: **What changed in the files?**

The changelog answers: **What materially changed in the system, why did it change, and what should future work assume because of it?**

## Required agent behavior

Before completing any work that changes repository files, every agent must evaluate whether the changelog needs an update.

The agent must choose one of two outcomes:

1. **Update `CHANGELOG.md`** because the work contains a meaningful change.
2. **Do not update `CHANGELOG.md`** because the work is routine, corrective, or too minor to matter in the repository's evolution.

Do not ask Keith whether to update it. Make the decision automatically using this standard.

A task is not complete until this evaluation has happened.

## Decision-density heuristic

Ask:

> If someone reviewed this repository six months from now, would knowing this change help them understand how the system, project, or operating model evolved?

If yes, record it.

If Git history alone is sufficient, do not add a changelog entry.

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
- A new standard or convention that changes future work

## Usually do not record

- Typos, formatting, and link fixes
- Routine maintenance with no durable effect
- Minor wording improvements that preserve meaning
- Intermediate drafts that do not change direction
- Mechanical file moves that do not change structure or interpretation
- Routine refactoring
- Generated-content refreshes with no material change
- Merge-only commits
- Every commit or every session

## How to write an entry

A strong entry should answer three questions:

1. What changed?
2. Why did it change?
3. What should future work do differently because of it?

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

### Weak example

```markdown
### Added
- Added Mission Control documentation.
```

### Strong example

```markdown
### Decided
- Introduced Mission Control as the operational control surface for active work, while keeping GitHub as durable knowledge and Google Drive as the home for active working documents.
```

## Relationship to other history files

- `CHANGELOG.md` records the executive evolution of the repository.
- Git commits preserve the exact technical and file history.
- `docs/build/DECISIONS.md` records durable decisions and rationale.
- `MEMORY.md` records what is active and true now.
- `docs/journal/HANDOFF.md` records session narrative and next steps.
- `docs/journal/archive.md` preserves retired working context.

Do not duplicate full rationale across these files. Link to the relevant decision or project document when useful.

## Definition of done

Before reporting completion, every agent must check:

- Did this work materially change what the repository is, how it operates, or what future work should assume?
- Did a project or program meaningfully start, change, pause, complete, or end?
- Did canonical guidance or AI behavior change?
- Would future Keith benefit from seeing this in the repository's executive history?

If yes, update `CHANGELOG.md` in the same branch or pull request.
