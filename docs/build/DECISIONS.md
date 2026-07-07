# Decisions

This document records important product, content, architecture, and platform decisions along with the rationale behind them.

---

### 2026-06-07: Use owned canonical resources as the platform hub

Decision:
Aspirationalist will prioritize owned canonical resources and topic hubs as the durable center of the platform.

Rationale:
The most likely acquisition path is distributed content across LinkedIn, newsletter, Substack, video, and other channels. Those channels should point back to durable owned resources that can be updated, improved, bundled, gated, monetized, and connected to community or future apps.

Consequences:
- The initial site structure prioritizes Resources and Topics over Articles.
- Long-form articles may remain external or secondary in v1.
- The site becomes the source of truth for key artifacts, frameworks, guides, and tools.
- I should start with canonical resources, not posts on social media sites

---

### 2026-06-07: Adopt Next.js + Sanity + Vercel as the core stack

Decision:
Build Aspirationalist on Next.js (frontend), Sanity (CMS), and Vercel (hosting).

Rationale:
This is the most common modern content/platform stack. It has strong AI tool support (Cursor, Claude, Codex), a clean separation between content editing and code, and scales from a content site into web apps without a rewrite. Sanity gives non-engineers a UI for publishing content without touching code. Vercel gives one-click deploys from GitHub with preview URLs per branch.

Framer was considered as a faster no-code alternative for v1 but rejected in favor of long-term flexibility and compatibility with the agent-assisted build workflow.

Consequences:
- Next.js is the frontend framework. Do not propose alternatives.
- Sanity is the CMS. Content types should be defined as Sanity schemas.
- Vercel is the hosting and deployment platform.
- GitHub remains the source of truth for code and docs.
- Supabase is the likely database when auth, gating, or user data is needed.

---

### 2026-06-07: Move repository outside OneDrive

Decision:
Store the repository at `C:\dev\Aspirationalist`.

Rationale:
OneDrive synchronization created Git lock conflicts that interfered with AI-assisted development workflows. The `.git` folder requires exclusive file access during commits, which OneDrive's continuous sync process disrupts.

Consequences:
- All local development, GitHub Desktop, Claude, Cursor, and other tools should use `C:\dev\Aspirationalist` as the working copy.
- `C:\dev` is outside OneDrive and will not be synced automatically.
- GitHub remains the remote backup and source of truth.

---

### 2026-06-07: Use shared agent instructions with tool-specific adapters

Decision:
Use `AGENTS.md` as the shared repo-level instruction file for AI agents, with tool-specific adapter files such as `CLAUDE.md` and `.cursor/rules/project.mdc` pointing back to it.

Rationale:
Aspirationalist is intended to be built with multiple AI tools over time, including Claude, Codex, Cursor, Gemini, and future coding agents. A shared instruction file keeps product direction, workflow expectations, and agent behavior consistent across tools while reducing repeated prompting.

Consequences:
- `AGENTS.md` becomes the central source of truth for agent behavior.
- Tool-specific files should stay lightweight and point back to `AGENTS.md`.
- Future agent integrations should be configured to read or follow `AGENTS.md`.
- Changes to agent behavior should usually be made in `AGENTS.md` first.

---

### 2026-07-07: Use Artifact as the canonical content object

Decision:
Use `Artifact` as the internal term for a polished, shareable output that delivers standalone value to another person.

Projects are active workspaces. They use Sources and Working Documents to develop Canonical Material and produce Artifacts. Topics group related Projects and Artifacts for discovery.

Rationale:
`Artifact` tells Keith that an output is intended to leave the workspace and be useful to someone else. `Resource` had become ambiguous because it could also describe private reference material.

Consequences:
- The internal content model uses `Artifact` instead of `Resource`.
- The normal development path is `source → working → canonical → artifact`.
- Topic pages link to Projects and Artifacts instead of duplicating files.
- Existing topic folders remain until a deliberate migration is approved.
- The public site may still use `Resources` as a navigation label if that is clearer to visitors.

---

### 2026-07-07: Work publicly and candidly by default

Decision:
Aspirationalist projects, notes, decisions, mistakes, drafts, and internal reasoning may be public by default.

Confidentiality is handled as a specific boundary. Material is excluded or redacted when Keith does not have the right to share it, or when it exposes private information about someone else.

Rationale:
Keith is highly transparent and candid. The inner workings of a project can be useful content and evidence of how expertise develops. Unpolished or critical material is not automatically confidential.

Consequences:
- Agents preserve useful unfinished thinking and decision history.
- Agents do not sanitize work merely because it reveals mistakes or uncertainty.
- Agents flag specific confidentiality concerns instead of making an entire project private by default.
- Keith retains final judgment about what he publishes.

---

### 2026-07-07: Require pull requests for main

Decision:
Protect the `main` branch and require repository changes to arrive through a pull request.

Rationale:
Multiple AI agents may work in the repository. Pull requests create a consistent review checkpoint before changes become canonical.

Consequences:
- Agents create a branch for repository changes.
- Agents open a pull request and summarize what Keith should review.
- Direct commits to `main` are blocked.
- Keith merges after reviewing the changed files.
