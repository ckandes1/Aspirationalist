# Docs Map

This is a map. It points to where things live and how they connect. It does not restate their content. For the rules agents follow, read `AGENTS.md`. For what is active right now, read `MEMORY.md`.

## How the systems connect

**Vision OS** turns a long-term vision into weekly execution. Its chain is vision, candidate hypotheses, one bet, a 30 to 90 day scope, weekly reflection, and daily time blocks.
- Framework: `projects/vision-os/canonical/operational-blueprint.md`
- Overview: `projects/vision-os/README.md`

**The Idea Murder Machine** is the filter between candidate hypotheses and the one bet. Gate One is its first stage, five questions an idea must pass before any planning starts.
- Detail: `projects/vision-os/canonical/gate-one.md`
- Originals: `projects/vision-os/source/`

**The project charter** is where Vision OS meets real work. Every project README opens with one. The rules are in `AGENTS.md` and the reasoning is in `build/DECISIONS.md`.

**MQ Package and AR Advisory GTM** are two projects with a boundary. The MQ Package holds reusable MQ methods, tools, and canonical guidance. AR Advisory GTM holds buyer research, offer hypotheses, and commercial learning.

**How material matures:** `source → working → canonical → artifact`. External tools such as NotebookLM can hold material before it enters the repository. GitHub is authoritative once material has been processed in.

## Where things live

| Location | What it holds |
|---|---|
| `AGENTS.md`, `KEITH.md` | Agent rules and Keith's working style |
| `MEMORY.md` | What is active and true now |
| `CHANGELOG.md` | Executive history of the repository |
| `projects/` | Active workspaces with sources, working documents, canonical material, and artifacts |
| `personal/` | Work outside the platform, using the same structure as `projects/` |
| `topics/` | Groups of related projects and artifacts, plus raw notes |
| `product/` | Product direction: audience, content model, strategy, information architecture, PRD, site vision |
| `build/` | Architecture, build workflow, and `DECISIONS.md` |
| `standards/` | Conventions agents follow, currently the changelog standard |
| `journal/` | Session handoffs and archive |
| `../skills/` | Reusable agent workflows |

## Projects

- `projects/vision-os/`: the vision-to-execution system and the Idea Murder Machine
- `projects/mq-package/`: reusable documentation and workflow for the Gartner Magic Quadrant cycle
- `projects/ar-advisory-gtm/`: validating an independent Analyst Relations advisory offer
- `projects/freelance-campaign/`: not described here because it had not been reviewed when this map was written. Read its README.

## Before placing new work

1. Check this map and `MEMORY.md` for an existing home.
2. Check whether the work is a stage or part of an existing project before proposing a new one.
3. Apply the recognition rules in `AGENTS.md` only after the first two checks.
