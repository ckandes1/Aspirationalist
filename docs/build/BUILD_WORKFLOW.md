# Build Workflow

## Purpose

Define how Aspirationalist should be built, reviewed, documented, and deployed over time.

## Working Model

GitHub is the source of truth.

The repo should contain product docs, content strategy, build decisions, code, changelog, and agent instructions.

AI tools such as Claude, Codex, Cursor, Gemini, or future coding agents should work from the repo and update the repo.

## Default Workflow

1. Define the task and identify its source-of-truth documents and approval scope.
2. Create or update relevant product/build documents using existing conventions.
3. Make proposed changes on a branch.
4. Open a pull request with the **Decision brief** required by `AGENTS.md`: action, material change, evidence, risks, recommendation and exact approval boundary.
5. Classify the risk. Request a distinct AI review for high-impact strategy, canonical research, major dependency, or security/privacy changes where feasible; disclose any review limitations.
6. Review preview deployments when the change affects deployed software, and attach relevant observed checks.
7. Keith reviews and merges only when the stated scope is acceptable. A raw-source capture PR archives source material; it does not approve its underlying claims.
8. Record durable decisions, changelog changes and session state where required.

## Why this is lightweight

The decision brief is the front-facing interface to underlying evidence and drafts. Additional orchestration services, dependency dashboards and cross-provider protocols are deferred until repeated work demonstrates a real gap.

## Principle

No AI tool is the long-term memory for the project.

The repo is the memory.
