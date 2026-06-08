# Content Model

## Purpose

Define what a Resource is, what types exist, what fields each has, and how Resources relate to other content on the site.

This document gates stack and CMS decisions. Do not select a framework or content management approach until this is stable.

---

## Core Concept: The Resource

A Resource is any owned artifact that delivers direct, standalone value to a reader.

Resources are the primary unit of content on Aspirationalist. They are durable, linkable, updatable, and can be bundled, gated, or monetized over time.

A Resource is not a blog post. It is not a social media update. It is a canonical artifact that lives on the site and does not expire.

---

## Resource Types

| Type | Description | Examples |
|---|---|---|
| Guide | Explains how to do something, step by step | How to run a Gartner briefing, how to build as a non-coder |
| Framework | A mental model, structure, or system for thinking about a problem | Corporate thesis framework, market intelligence framework |
| Template | A reusable, fillable artifact | Analyst briefing template, PMM one-pager template |
| Checklist | A scannable list for completing or auditing something | AR program checklist, launch readiness checklist |
| Playbook | A comprehensive end-to-end operational guide | Full AR playbook, AI agent workflow playbook |
| Explainer | Defines and contextualizes a concept | What is analyst relations, what is a corporate thesis |
| Resource List | A curated collection of tools, links, or references | Best AI agent tools, recommended AR reading |

New types can be added as needed. Type is a tag, not a hard category — a resource can be both a Template and a Guide.

---

## Resource Fields

### Required

| Field | Description |
|---|---|
| Title | Clear, descriptive name |
| Slug | URL-safe identifier (e.g. `gartner-briefing-guide`) |
| Type | One or more resource types from the list above |
| Topic | One or more topics this resource belongs to |
| Summary | One to three sentence description of what the resource is and who it helps |
| Body | The resource content itself |
| Published date | When it was first published |

### Optional

| Field | Description |
|---|---|
| Updated date | When it was last meaningfully revised |
| Gated | Boolean — whether the resource requires email or account to access |
| Downloadable | Boolean — whether a file download is available (PDF, DOCX, etc.) |
| Related resources | Links to other resources on the site |
| Related topics | Additional topic associations beyond the primary topic |
| CTA | Call to action at the end (newsletter, community, related resource) |
| Status | Draft, Published, Needs Update |

---

## Default Access Model

Resources are free and open by default.

Some resources may be gated behind an email signup or free account. Gating is opt-in per resource, not a site-wide policy.

Paid resources are possible in the future but are not in scope for v1.

---

## Topics

Topics are the organizing hubs that group Resources by subject area.

A Resource belongs to at least one Topic. It may belong to more than one.

Initial topics:
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

```
Topic
  └── has many Resources

Resource
  └── belongs to one or more Topics
  └── may relate to other Resources
  └── may belong to a Project
```

---

## Open Decisions

- Whether Resources need versioning (e.g. v1, v2 of a template)
- Whether downloadable file formats are supported in v1 or later
- Exact gating mechanism (email capture vs. free account)
- Whether a Resource can be part of a Bundle (multiple resources sold or gated together)

---

## Out of Scope for v1

- Paid resources
- Resource bundles
- Comments or user-generated content
- Resource ratings or reviews
