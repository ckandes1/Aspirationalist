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
