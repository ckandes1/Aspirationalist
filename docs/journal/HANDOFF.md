# Aspirationalist Handoff

Session narrative for resuming work. Read `AGENTS.md` and `MEMORY.md` first for active context.

---

## Session Handoff — 2026-07-07

### Completed this session

- Audited the existing Aspirationalist repository and current topic structure.
- Confirmed that the MQ Package should live inside Aspirationalist as a project rather than as a separate repository.
- Clarified the model:
  - Projects are active workspaces.
  - Artifacts are shareable outputs intended to deliver practical value.
  - Topics are discovery and context layers that group related Projects and Artifacts.
- Chose `Artifact` as the internal term instead of `Resource` because it clearly signals that the output is intended to be shared and used.
- Established the default publishing stance: public and candid by default, with confidential material handled as a separate and specific boundary.
- Protected the `main` branch so changes must go through pull requests.
- Tested the rule successfully. GitHub rejected a direct write to `main`.
- Created branch `artifact-first-workflow` and updated the repo instructions, content model, content strategy, decisions, memory, and this handoff.

### MQ Package direction

The MQ Package is intended to become Keith's canonical operating system for running Gartner MQ season from end to end.

The project will begin with source documents, especially one mostly comprehensive file that consolidates Keith's candid notes and lessons from the 2026 MQ cycle. That source file should have:

1. A concise, usable synthesis at the top
2. The fuller rough notes and supporting material below

The canonical package will be developed from those source documents. Shareable Artifacts may later include a public-facing playbook or book, worksheets, quicksheets, templates, training decks, and distributed content.

### Immediate next actions

1. Review pull request for branch `artifact-first-workflow`.
2. Merge it if the definitions and rules are correct.
3. Create the minimal project shell under `docs/projects/mq-package/`.
4. Build the consolidated `source/2026-mq-season-notes.md` document before drafting the canonical playbook.
5. Reference existing Zone 1 / Zone 2 notes rather than duplicating them.

### Guardrails

- Make changes in small, reviewable increments.
- Do not move or migrate existing topic files until the new project structure is proven useful.
- Do not create empty folders for future work.
- Preserve candid process detail unless it is genuinely confidential or Keith does not have the right to publish it.

### To resume with an AI agent

Say: `Read AGENTS.md, MEMORY.md, and docs/journal/HANDOFF.md. Then continue the MQ Package project from the next uncompleted action.`

---

*Previous sessions archived in `docs/journal/archive.md`.*
