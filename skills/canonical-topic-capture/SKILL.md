---
name: canonical-topic-capture
description: Turn Keith's stream-of-consciousness insight, experience, or learning into repository-ready raw topic material without prematurely turning it into canonical guidance. Use when Keith asks to save something for later, preserve raw material, document a potential canonical topic, or capture a situation, pain, and emerging solution.
---

# Canonical Topic Capture

Use this skill when Keith has articulated an experience or learning that may later become a framework, artifact, or canonical topic.

The goal is to preserve the useful thinking in a form that can mature later. Do not force the material into a finished framework before the idea has been tested or developed.

## First decision: where does it belong?

Read `AGENTS.md`, `KEITH.md`, `MEMORY.md`, and the relevant topic or project README before writing.

Classify the material as one of these:

- **Topic raw note:** an experience, opinion, learning, or early model that may develop over time.
- **Project source:** material collected for a defined project with a specific outcome.
- **Working document:** synthesis, planning, decisions, or structure developed from existing sources.
- **Artifact draft:** a complete output intentionally designed for another person to use.

When the idea begins with Keith's lived experience and has not yet been developed into a named method, prefer a dated topic raw note.

Use one primary home. Link elsewhere later instead of copying the material.

## Choose the topic deliberately

Use an existing topic when it reasonably fits. Avoid creating a narrow topic for a single note.

Use `Personal Field Notes` when the material begins as a personal experience or learning and may later feed a broader topic or framework.

Create a new topic only when the material clearly represents a durable subject area that is likely to hold multiple notes, frameworks, projects, or artifacts. A new topic requires a README explaining its scope and intended direction.

## Capture structure

Use the following structure when it fits the material:

```markdown
# Working title

Status: Raw topic note, not canonical guidance  
Captured: YYYY-MM-DD  
Potential direction: Brief description of what this may become

## Core learning

State the emerging conclusion in one or two direct paragraphs.

## Situation

Describe what Keith was trying to do and the context that produced the learning.

## Pain or tension

Preserve the actual felt problem. Explain what was missing, confusing, ineffective, or directionless.

## What changed

Describe the realization, evidence, or mechanism that changed the understanding of the problem.

## Emerging system or solution

Capture the current proposed method in enough detail to be useful. Label assumptions, hypotheses, and unresolved choices.

## Proposed practice

Describe how the idea might be applied repeatedly in real life.

## Open questions

Preserve what still needs to be tested, clarified, named, or integrated.

## Raw language worth preserving

Include a small number of Keith's phrases when the wording contains useful emotional truth, stakes, or conceptual precision.
```

Use only the sections the material needs. Structure should make the note retrievable and usable without making it look more settled than it is.

## Editing rules

- Preserve the sequence from lived experience to learning.
- Keep the pain and stakes. Do not reduce the note to generic advice.
- Separate observation, interpretation, hypothesis, and proposed practice.
- Preserve meaningful uncertainty and contradictions.
- Do not invent examples, evidence, names, or outcomes.
- Keep Keith's specific distinctions and mechanisms.
- Clean transcription errors and repetition that add no meaning.
- Retain repetition when it reveals emphasis or an unresolved constraint.
- Apply `skills/keith-writing-style/SKILL.md`.
- Use dated filenames such as `YYYY-MM-DD-descriptive-slug.md`.

## Promotion rule

A raw note can move toward a framework when:

1. the central mechanism is clear;
2. the idea has been tested against experience or evidence;
3. important variants and failure modes are understood;
4. the concept can be named without overstating certainty; and
5. Keith deliberately approves the promotion.

Do not silently promote raw material into canonical guidance.

## Repository workflow

1. Create a branch.
2. Add or update the relevant topic README only when needed.
3. Create the dated raw note.
4. Update repository memory or handoff files when the capture changes active direction or creates a reusable workflow.
5. Open a pull request that explains the placement, the maturity level, and what remains unresolved.
