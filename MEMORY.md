# Memory

Active working context. Kept under 275 lines. When it exceeds that, completed items move to `docs/journal/archive.md`.

---

## Active Work

- The MQ Package is the current anchor project.
- The immediate goal is to consolidate Keith's scattered 2026 MQ season notes into one candid, contextual source document.
- That source document will support a canonical MQ operating system and later shareable Artifacts such as a book, worksheets, quicksheets, templates, training decks, and distributed content.
- Branch `artifact-first-workflow` updates the repo vocabulary, project model, transparency rules, and pull request workflow.
- After that branch is reviewed and merged, create the minimal MQ Package project shell under `docs/projects/mq-package/`.
- Existing Zone 1 / Zone 2 notes remain useful source material and should be referenced rather than duplicated.
- Next.js + Sanity + Vercel stack is decided, scaffolding has not started.

## Recent Decisions

- **Artifact:** internal term for a polished, shareable output intended for someone else to use.
- **Project:** active workspace that turns Sources and Working Documents into Canonical Material and Artifacts.
- **Topic:** discovery and context layer that groups related Projects and Artifacts.
- **Transparency:** public and candid by default; confidentiality is a separate, specific boundary.
- **Git workflow:** `main` is protected and changes must arrive through pull requests.
- **Content strategy:** build useful canonical Artifacts first, then derive distributed content from them.

## Open Questions

- Exact minimal folder structure for the MQ Package project after the terminology PR is merged
- Final structure of the consolidated 2026 MQ season notes source document
- Whether the public website navigation label remains `Resources` or changes later
- Newsletter platform
- Community platform
- Auth provider
- Payment provider and gated Artifact model
- Whether Articles become a primary nav item in v1
