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

## Build a fidelity map before drafting

Before organizing or rewriting the source, identify these elements privately:

1. **Central tension:** What seems contradictory or surprising about the experience?
2. **Felt experience:** What words describe how it actually felt, such as messy, directionless, stuck, overwhelmed, or ineffective?
3. **Causal chain:** What happened, why did it create that feeling, what was missing, and how did the realization emerge?
4. **Repeated emphasis:** Which ideas or phrases did Keith return to several times?
5. **Missing mechanism:** What connection, structure, feedback loop, measurement, or decision process was absent?
6. **Emerging solution:** What system or practice is currently being proposed?
7. **Uncertainty:** What remains untested, unresolved, or easy to overstate?

The note must preserve the causal chain, not only the conclusion or proposed system.

A useful test is whether a reader could explain:

- why Keith felt the way he did;
- why the existing approach was insufficient;
- which missing mechanism caused the problem; and
- how the proposed system addresses that mechanism.

## Capture structure

Use the following structure when it fits the material:

```markdown
# Working title

Status: Raw topic note, not canonical guidance  
Captured: YYYY-MM-DD  
Potential direction: Brief description of what this may become

## Core learning

State the emerging conclusion and the central tension directly.

## Situation

Describe what Keith was trying to do and the context that produced the learning.

## Why it felt this way

Preserve the causal chain between the situation and the felt problem. Make the missing structure, tracking, feedback, connection, or evidence explicit.

## Pain or tension

Preserve the actual felt problem and the language Keith used to describe it.

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

## Original source capture

Preserve the original submission in a collapsible appendix or link to a separate source file.
```

Use only the sections the material needs. Structure should make the note retrievable and usable without making it look more settled than it is.

## Source preservation

For a substantial stream-of-consciousness capture, preserve the original submission by default.

Preferred options:

1. Include it at the bottom of the raw note inside a GitHub `<details>` section.
2. Create a separate dated source file when the capture is very long, contains multiple sessions, or will be reused by several working documents.
3. Use selective excerpts only when the full source is already preserved elsewhere and linked clearly.

The synthesized note is an interpretation. The source record lets Keith or a future agent verify what was emphasized, recover details that were compressed away, and revise the interpretation later.

Do not duplicate the same source across multiple files. Preserve it once and link to it.

## Editing rules

- Preserve the sequence from lived experience to learning.
- Keep the pain and stakes. Do not reduce the note to generic advice.
- Preserve the central tension even when it appears logically inconsistent at first.
- Make causal language explicit: because, therefore, which meant, and as a result.
- Treat repeated words and ideas as signals of importance before removing repetition.
- Separate observation, interpretation, hypothesis, and proposed practice.
- Preserve meaningful uncertainty and contradictions.
- Do not invent examples, evidence, names, or outcomes.
- Keep Keith's specific distinctions and mechanisms.
- Clean transcription errors and repetition that add no meaning.
- Retain repetition when it reveals emphasis or an unresolved constraint.
- Apply `skills/keith-writing-style/SKILL.md`.
- Use dated filenames such as `YYYY-MM-DD-descriptive-slug.md`.

## Fidelity review before committing

Compare the finished note against the original source and check:

- Is the central tension visible near the top?
- Does the note explain why the feeling occurred, rather than merely naming the feeling?
- Are the words Keith repeated or emphasized represented in the synthesis?
- Did structure, tracking, measurement, feedback, or connection disappear during cleanup?
- Can the reader follow the full cause-and-effect chain?
- Did the proposed solution crowd out the experience that produced it?
- Is any sentence cleaner or more certain than the source supports?
- Is the original source preserved or linked?

When an important detail is difficult to integrate cleanly, keep it in the raw note. Raw capture prioritizes fidelity over elegance.

Keith should still review each raw capture. The skill reduces predictable loss during synthesis, while Keith's review remains the final fidelity check.

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
3. Create the dated raw note and preserve the original source.
4. Run the fidelity review against the source.
5. Update repository memory or handoff files when the capture changes active direction or creates a reusable workflow.
6. Open or update a pull request that explains the placement, the maturity level, and what remains unresolved.
