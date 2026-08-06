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

---

### 2026-07-08: Capture potential canonical topics as structured raw notes

Decision:
When Keith shares an experience, insight, or stream-of-consciousness learning that may become canonical later, capture it first as a dated raw topic note using `skills/canonical-topic-capture/SKILL.md`.

The raw note should preserve the situation, felt pain, emerging mechanism, proposed solution, and unresolved questions. It should remain visibly non-canonical until Keith deliberately develops and approves it as a framework or project.

Rationale:
Keith frequently develops useful ideas through verbal reflection but does not consistently document them. Moving directly from dictation to polished guidance can remove the pain that made the insight meaningful and harden an early hypothesis before it has been tested.

Consequences:
- Agents use the canonical topic capture skill when Keith asks to save raw material for later.
- Personal experiences default to `Personal Field Notes` when no more specific established topic fits.
- New topics are created only for durable subject areas likely to contain multiple notes, frameworks, projects, or artifacts.
- Raw notes keep one primary home and may be linked elsewhere later.
- Promotion from raw material to framework or canonical guidance requires deliberate review.

---

### 2026-07-14: Use external workspaces for pre-structure source intake

Decision:
Use external tools such as NotebookLM as intake and exploration workspaces for source material that has not yet been converted into the repository's structured content model.

GitHub remains the source of truth. Once material is reviewed and converted into structured project or topic material, it must have one primary home under the appropriate `source`, `raw`, `working`, `frameworks`, `canonical`, or `artifacts` directory.

Rationale:
Some source assets are easier to collect, search, compare, and explore in tools designed for unstructured material. These tools support the work before the material is mature enough for the repository. Treating an external workspace as canonical would create competing sources of truth and make it unclear which material has been reviewed, approved, or incorporated.

Consequences:
- External workspaces may hold transcripts, decks, notes, prompts, drafts, research, and exploratory synthesis.
- External summaries and AI-generated output remain non-canonical until deliberately processed into GitHub.
- Each project or topic may document its specific intake workspace and processing queue.
- Structured material keeps one primary home in the repository.
- Public content and reusable artifacts are derived from the repository's canonical material.
- Automated synchronization is deferred until the intake and processing workflow is stable.

The MQ Package is the first active implementation of this workflow through the NotebookLM project `"MQ Package" Content for Aspirationalist`.

---

### 2026-07-26: Separate personal projects by path

Decision:
Work that is not Aspirationalist, including real estate, household, family, and personal finance, lives under `docs/personal/<project-name>/`, using the same structure and maturity path as `docs/projects/`. The path is the only marker. No `personal:` or `context:` field is added anywhere.

`docs/projects/` remains the default. `docs/personal/` is used only when a project clearly sits outside the platform.

Rationale:
Personal work needs the same discipline as platform work, and the same agent instructions already describe that discipline. Duplicating the system for personal use would create two conventions to maintain. Adding a metadata field instead of using the path would create a second source of truth that can drift out of sync with where the file actually sits.

Making `docs/projects/` the default rather than requiring an explicit choice means agents only exercise judgment in the minority of cases, which is where judgment is actually needed.

Consequences:
- Agents ask rather than guess when classification is genuinely ambiguous.
- Agents do not move projects between the two locations without approval, because reclassification breaks links.
- Thinking from a personal project that is useful publicly is written as an artifact under the relevant topic and linked back, rather than by relocating the project.
- The repository remains public and the existing transparency rules apply unchanged. Personal projects encounter third-party and financial specifics more often, so agents flag the specific passage, such as addresses, account numbers, counterparty names, and figures, rather than making a whole project private.
- Personal projects appear in `MEMORY.md` under the same headings as everything else.

---

### 2026-07-26: Require a project charter and surface project candidates

Decision:
Every project README opens with a charter: vision link, active hypothesis, kill criteria, 30–90 day scope, and status. The charter is the applied form of `docs/projects/vision-os/canonical/operational-blueprint.md`.

Agents may draft the vision link, scope, and status. Agents do not write the hypothesis or the kill criteria.

Separately, agents raise the possibility of a project when one of four conditions appears: work with an outcome that outlasts the session and has no project, a topic `raw/` folder with three or more notes on the same problem, real work with no home in the repo, or an existing project with unfilled charter `TODO`s or a stale status date.

Rationale:
The Vision OS blueprint was canonical but unapplied. No project in the repository carried a hypothesis or anything that could end it, which meant projects could only be continued, never disproven. The charter is the enforcement point that connects the framework to actual work.

The recognition triggers exist because a charter requirement alone is passive. It depends on Keith remembering to invoke it. Agents already read this repository at the start of a session, so they are in position to notice when work has become a project and put the choice in front of him while it is live.

Agents are barred from writing the hypothesis and kill criteria because those are a decision about what Keith is willing to be wrong about. An agent producing them would be pattern-matching on nearby text, and the output would read as decided when nothing had been decided.

Consequences:
- One active hypothesis per project, no more than three active priorities repository-wide. A fourth surfaces as a conflict rather than being absorbed.
- Unanswered charter fields stay as explicit `TODO`s naming what is missing.
- When evidence trips a project's kill criteria, agents say so and add it to Open Questions in `MEMORY.md` rather than continuing to execute.
- Work without a charter stays in the relevant topic's `raw/` rather than becoming a project.
- Agents surface project candidates in one sentence and do not create the project themselves.
- The MQ Package and Vision OS both currently lack complete charters. Both are tracked in Open Questions.

---

### 2026-07-26: Separate AR offer discovery from campaign execution

Decision:
Create `docs/projects/ar-advisory-gtm/` as the project for validating an independent Analyst Relations advisory offer and its route to market.

Begin with structured buyer research and a limited number of free advisory engagements. Keep the paid offer, pricing, free asset, and campaign execution unresolved until real situations show which problem, method, output, and outcome are repeatable and valuable.

Keep the MQ Package as the primary home for reusable MQ methods, tools, and canonical guidance. Store buyer research, offer hypotheses, funnel design, campaign planning, and commercial learning in AR Advisory GTM.

Rationale:
The work began with a content campaign and funnel before the service itself was clear. Attempts to specify the paid offer from general expertise created false precision because Keith has not yet applied this knowledge as an external advisor in a real client situation.

Keith already has strong subject-matter credibility and prior inbound interest. The missing evidence is how that expertise changes a company's decisions and what a buyer would value enough to purchase. A small discovery phase is the fastest way to learn that while providing genuine help.

Consequences:
- The project follows `market opportunity → buyer problem → desired outcome → offer → evidence → message → route to market → campaign → learning`.
- Campaign execution remains paused during buyer and offer discovery.
- Free engagements are genuine help and research, not incomplete paid engagements or hidden upsells.
- Buyer interviews and free advisory work may run in parallel with MQ Package development because they can identify real needs and package gaps.
- Reusable MQ methods and artifacts are developed in the MQ Package and linked into AR Advisory GTM.
- The AR Advisory GTM charter keeps the active hypothesis and kill criteria as explicit `TODO`s for Keith.

---

### 2026-07-26: Require merge-ready handoff text from AI agents

Decision:
After an AI agent opens or updates a pull request, its user-facing handoff must include a ready-to-paste suggested merge title and suggested merge description for the complete current pull request.

The title uses imperative tense, stays under 72 characters, and begins with the agent name in square brackets. The description summarizes the full pull request rather than only the latest commit.

Rationale:
Keith reviews and merges AI-generated pull requests manually. GitHub may ask him to enter or edit the final merge or squash commit title and description. Requiring him to return to the agent for that text creates repeated avoidable work, especially when the agent already has the best context on the complete change.

Consequences:
- Every AI handoff after repository changes uses the headings `Suggested merge title` and `Suggested merge description`.
- The suggested text is ready to paste into GitHub.
- Updating an existing pull request requires refreshing the suggestion to cover the entire pull request.
- The term `pull request` refers to the review package; Keith's final action is to merge the pull request into `main`.