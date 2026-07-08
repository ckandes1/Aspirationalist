# Operational Blueprint: Vision-to-Hypothesis Validation Engine

## 1. Executive Summary

This document serves as the operational framework for translating a macroscopic, long-term vision into daily, time-blocked execution. The core objective is to eliminate the friction of feeling "directionless" by establishing intermediate scaffolding between high-level strategy (the Vision Deck) and daily tasks.

This system treats execution as a Hypothesis Validation Engine. Instead of scoping massive projects, a vision is mapped to multiple potential solutions (hypotheses). The single quickest, most testable hypothesis is selected, bound to a strict 30-to-90 day validation scope, and filtered through the Idea Murder Machine. If it fails to clear its prerequisite thresholds, it is systematically eliminated.

---

## 2. The Architecture

```
[Vision Deck]                --> Macro impact goals (Max 3 active priorities)
       |
       v
[Idea Murder Machine]        --> Sandbox of potential testable paths
       |
       v
[ONE Hypothesis]             --> Chosen, quickest-to-test path (Max 1 per priority)
       |
       v
[30-to-90 Day Bound Scope]   --> Strict boundary line to prove/disprove the hypothesis
       |
       v
[Weekly Reflection Loop]     --> Core audit: Review Deck & One-Pager, set weekly time blocks
       |
       v
[Daily Tasks]                --> Outcome-focused deliverables within isolated time blocks
```

---

## 3. Active Priority Template (Hypothesis Validation Sheet)

*For each of the active priorities, spin up a section or file using this structure.*

### A. The Vision
<!-- What macro-level impact is this priority driving toward? Reference your Vision Deck items here. -->

### B. The Active Hypothesis
<!-- What is the specific, testable solution being bet on right now? Why is it the fastest or easiest to validate? -->

### C. Prerequisite Thresholds ("Murder" Criteria)
<!-- What must prove true during this short-term window for this path to remain viable? What kills the idea? -->

### D. The 30-to-90 Day Bound Scope
<!-- What is the exact, time-bound artifact or outcome being delivered to test the hypothesis this quarter? -->

### E. Weekly Reflection Protocol

*Every week, execute a 15-minute reflection block to prepare for the upcoming week:*

1. **Past Week Review:** Did I deliver the outcome promised in my time blocks? If not, what was the friction point?
2. **Vision Deck Alignment:** Does this path still align with the broader macro goals?
3. **Next Week Time-Block Focus:** What is the singular concrete deliverable for next week's execution blocks?

---

## 4. Initialization Prompt for Claude

*Copy and paste this text into your Claude project to begin:*

"Claude, initialize the Idea Murder Machine framework using this framework document as our source of truth. We are setting up an execution system for my repository.

I have a Vision Deck and need to maintain a strict limit of 3 or fewer active priorities. I want you to help me ingest my raw thoughts and run them through Section 3 (The Hypothesis Validation Sheet) so I can define my very first 30-to-90 day bound scope and set up my weekly reflection criteria. Let's begin parsing the first priority."
