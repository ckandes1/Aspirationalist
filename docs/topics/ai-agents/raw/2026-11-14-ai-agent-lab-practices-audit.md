# AI agent playbooks: applicability audit for Aspirationalist

**Captured:** 2026-11-14
**Status:** Research synthesis. This audit is a working document; only the decision-oriented review policy identified below has been explicitly approved by Keith. No futures project charter or new agent software is authorized.

## Executive conclusion

Keep the existing GitHub-native collaboration system. Adopt a concise **decision brief** at the top of each pull request and **risk-based independent AI review** for consequential changes. This is the first identified practical gap: the repository is capable of retaining detailed AI work, while the human director needs a reliable, low-effort interface to decide what enters the accepted body of work. Other agent-orchestration features remain optional until a concrete task requires them.

The decision brief is our application of established practices, **not** a claim that any laboratory has published the exact required template.

## Source audit

| Source | Relevant published practice | Fit with this repo | Recommended action |
|---|---|---|---|
| [OpenAI, Iterating Development Workflows with Codex](https://developers.openai.com/cookbook/examples/codex/iterating-development-workflows-with-codex) (2026-08-03) | Durable `AGENTS.md` instructions, optional planning/context files, small phases, approval and evidence | `AGENTS.md`, `MEMORY.md`, handoffs, PRs and project charters exist | Reuse. Avoid creating a parallel harness without need |
| [Anthropic, Building effective agents](https://www.anthropic.com/research/building-effective-agents) (2024-12-19; site flags evolving implementation guidance) | Begin with simple composable patterns; add routing, parallel workers and evaluator-optimizer loops only when justified | Existing human-managed assignments plus review can implement the essential practices | Use targeted AI criticism of significant work; defer autonomous orchestration |
| [Anthropic, How we built our multi-agent research system](https://www.anthropic.com/research/multi-agent-research-system) (2025-06-13) | Lead researcher delegates open-ended work, workers research independently, results are compressed into synthesis and evaluated | Strong potential fit for later large source reviews and competing world models | Pilot when a research assignment actually benefits from parallel agents |
| [OpenAI, A practical guide to building agents](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf) | Distinguish agent-suitable tasks, define guardrails, design human handoffs and escalation | Current approvals, project charter and PR boundaries already provide oversight | Use explicit human decision scope and evidence; defer bespoke runner |
| [Google, Developer's Guide to AI Agent Protocols](https://developers.googleblog.com/en/developers-guide-to-ai-agent-protocols/) (2026-03-18) | MCP/A2A and other protocols support cross-system tool and agent interoperation | The repository itself is vendor-neutral, and agents can use separate connectors to the same artifacts | Monitor; add protocol integration only if provider interoperability becomes a measured bottleneck |

**Freshness boundary:** These are architectural references as published. Product offerings and APIs change. Revalidate compatibility before selecting a framework, paid service or deployment.

## Gap analysis and recommendations, ranked

### 1. Keep current repository model. Status: implemented

- GitHub is authoritative for the structured, reviewed project record.
- `AGENTS.md` owns shared AI instructions; adapters for other AIs point to it.
- `MEMORY.md` and `docs/journal/HANDOFF.md` support new-context entry.
- Project charters, drafts, canonical material, decisions and PR review have defined ownership.
- The November 14 futures source capture is saved at `docs/topics/aspirationalism/raw/2026-11-14-ai-abundance-futures-project-handoff.md`.
- No evidence of a need for a custom work register, cross-vendor coordinator, autonomous scheduler or frontend exists yet.

### 2. Add decision-oriented review and risk-based second opinions. Status: approved direction, proposed implementation in this PR

**Decision brief (top of each material PR):**
- **Action requested:** Archive unreviewed source; approve a working approach; approve canon; change operating policy; or release an artifact.
- **What changed / why:** Two or three plain-language points.
- **Evidence and confidence:** Links to supporting files, sources, test/check results, and any limitations.
- **Risks / unresolved issues:** What remains untested, contradictory or dependent on another decision.
- **Recommendation and approval boundary:** Precisely what a merge authorizes, and what it does not.
- **Review assurance:** Self-review completed; independent AI review performed / pending / waived with reason. Name reviewer and show actual findings only if review occurred.

A one-page brief should usually be sufficient. Detailed work is reached through links. The brief is the interface to the evidence, rather than a replacement for it.

**Second-opinion trigger:** Seek an independent AI reviewer for changes that promote foundational ideology claims or fictional world rules into canon, substantially alter a project hypothesis/methodology, change privacy/security constraints, or have material downstream dependency impact. A contributor may request independent review for uncertain or contested research. Routine source capture, wording, and minor maintenance can use self-review.

**Decision rights:** Keith sets the hypothesis, kill criteria and major canon/strategic gates. A reviewer reports findings and recommendations. An AI's APPROVE status, completion summary or successful PR merge should never be used to imply that the underlying world thesis is proven.

**Specific lesson from PR #25:** Merging a source handoff stores and makes unreviewed research discoverable. It does not establish the ideology, civilization, or story canon.

### 3. Use scoped research assignments and optional parallel workers. Status: conditional

When Stage 0 is chartered, assign a bounded question with sources, alternatives, acceptance criteria, dependencies and review gate. For a genuinely broad research question, parallel AIs may investigate independently, and a reviewer synthesizes and challenges their work. Use GitHub Issues/PRs already available. Do not prescribe an always-on coordinator before actual volume warrants it.

### 4. Add dependency revalidation only when material. Status: defer implementation

When a canonical world assumption changes, note downstream affected research, chapters, timelines or plot rules. Initially record dependency links in the relevant document or issue. Dedicated graph software and change-propagation automation are options only if manual traces become costly or unreliable.

### 5. Dedicated director dashboard, orchestration service and agent protocol integration. Status: defer

These may eventually support a layered interface (project control → knowledge/canon → public artifacts), but require a demonstrated workload, measurable review friction, and a product design gate. First try the decision-brief format directly in GitHub.

## Stage 0 implications

The **future project architecture study** should evaluate ideology-first, world-first and iterative approaches; recover the aspiration-list source and previously cited Drive material; assess the proposed historical bookends; compare publishing formats; and map reviews/dependencies. It should incorporate decision briefs and appropriate independent critique as adopted workflow. It cannot create a project charter until Keith supplies the active hypothesis and kill criteria per `AGENTS.md`.

**Do not treat this lab-practices audit itself as the entire Stage 0 study.** It is the operating-method comparison that precedes the substantive futures-program architecture and research.

## Concrete acceptance checks for the review policy

1. A new PR has a short action/recommendation/approval-boundary brief with pointers to supporting evidence.
2. A future AI can tell whether the material is raw, working, canonical or public artifact.
3. High-impact changes record whether independent AI review actually happened and its substantive findings, or why it was not done.
4. An archive-only PR clearly says merging does not approve source claims.
5. No new orchestration app, protocol requirement or provider lock-in is introduced.

## Open questions

- Which changes beyond the stated high-impact examples need a mandatory second review? Start with judgment and refine from actual use.
- What should the first **Futures Project** hypothesis and kill criteria be? Keith owns these under current charter rules.
- Does the existing source material justify a new project now, or should the next assignment remain an Aspirationalism topic study?
