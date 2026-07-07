# Content Model

## Purpose

Define what an Artifact is, what types exist, what fields each has, and how Artifacts relate to Projects and Topics.

This document gates stack and CMS decisions. Do not select a framework or content management approach until this is stable.

---

## Core Concept: The Artifact

An Artifact is an owned, shareable output that delivers direct, standalone value to another person.

Artifacts are the primary unit of practical content on Aspirationalist. They are durable, linkable, updatable, and may be downloadable, gated, bundled, or monetized over time.

An Artifact may be a guide, framework, template, checklist, playbook, explainer, worksheet, training deck, or other useful output. The defining trait is that someone else can take it and use it.

`Artifact` is the internal content-model term. The public website may still use `Resources` as a navigation label if that is clearer to visitors.

---

## Artifact Types

| Type | Description | Examples |
|---|---|---|
| Guide | Explains how to do something, step by step | How to run a Gartner briefing, how to build as a non-coder |
| Framework | A mental model, structure, or system for thinking about a problem | Corporate thesis framework, market intelligence framework |
| Template | A reusable, fillable artifact | Analyst briefing template, PMM one-pager template |
| Checklist | A scannable list for completing or auditing something | AR program checklist, launch readiness checklist |
| Playbook | A comprehensive end-to-end operational guide | Full AR playbook, AI agent workflow playbook |
| Explainer | Defines and contextualizes a concept | What is analyst relations, what is a corporate thesis |
| Worksheet | A guided artifact that helps someone work through a decision or process | MQ pre-season planning worksheet |
| Training Deck | A presentation designed to teach or enable a group | Executive MQ training deck |
| Curated List | A selected collection of tools, references, or examples | Recommended AR reading, AI agent tools |

New types can be added as needed. Type is a tag, not a hard category. An Artifact may have more than one type.

---

## Artifact Fields

### Required

| Field | Description |
|---|---|
| Title | Clear, descriptive name |
| Slug | URL-safe identifier, such as `gartner-briefing-guide` |
| Type | One or more Artifact types from the list above |
| Topic | One or more Topics this Artifact belongs to |
| Summary | One to three sentence description of what the Artifact is and who it helps |
| Body | The Artifact content itself |
| Published date | When it was first published |

### Optional

| Field | Description |
|---|---|
| Updated date | When it was last meaningfully revised |
| Project | The Project that produced or maintains the Artifact |
| Gated | Whether the Artifact requires an email signup or account |
| Downloadable | Whether a file download is available, such as PDF, DOCX, PPTX, or XLSX |
| Related Artifacts | Links to other Artifacts |
| Related Topics | Additional Topic associations beyond the primary Topic |
| CTA | Call to action at the end, such as newsletter, community, or another Artifact |
| Status | Draft, Published, or Needs Update |
| Version | Current public version when versioning is useful |

---

## Default Access Model

Artifacts are free and open by default.

Some Artifacts may be gated behind an email signup or free account. Gating is opt-in per Artifact, not a site-wide policy.

Paid Artifacts are possible in the future but are not in scope for v1.

---

## Projects

Projects are active bodies of work that turn Sources and Working Documents into Canonical Material and Artifacts.

A Project may produce many Artifacts. A Project may also contain useful public process material that never becomes an Artifact, such as candid notes, decision history, or build journals.

Projects are defined and maintained under `docs/projects/`.

---

## Topics

Topics are discovery and context hubs that group related Projects and Artifacts by subject area.

An Artifact belongs to at least one Topic and may belong to more than one. A Project may also relate to more than one Topic.

Initial Topics:
- Analyst Relations
- Gartner
- Product Marketing
- Market Intelligence
- AI Agents
- Building as a Non-Coder
- Career Switching
- Aspirationalism
- Personal Field Notes

Topics are defined in full in `docs/product/INFORMATION_ARCHITECTURE.md`.

---

## Relationships

```text
Project
  ├── uses Sources and Working Documents
  ├── develops Canonical Material
  └── produces zero or more Artifacts

Topic
  ├── groups related Projects
  └── groups related Artifacts

Artifact
  ├── belongs to one or more Topics
  ├── may belong to a Project
  └── may relate to other Artifacts
```

A file should have one primary home. Topic pages link to Projects and Artifacts rather than duplicating them.

---

## Open Decisions

- Whether Artifacts need formal versioning in v1
- Whether downloadable file formats are supported in v1 or later
- Exact gating mechanism, such as email capture or free account
- Whether an Artifact can be part of a Bundle
- Whether the public navigation label should remain `Resources` or change later

---

## Out of Scope for v1

- Paid Artifacts
- Artifact bundles
- Comments or user-generated content
- Artifact ratings or reviews
