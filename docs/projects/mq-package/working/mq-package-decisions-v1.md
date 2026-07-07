# MQ Package Decisions v1

Status: Working document, not canonical guidance  
Created: 2026-07-07  
Primary source: `../source/2026-mq-season-notes.md`

## Purpose

This document converts the 2026 MQ source record into explicit working decisions for the MQ Package.

The source document preserves what happened, what I learned, contradictions, repeated concerns, and missing information. This document does something different: it states what the package should currently assume, what remains provisional, and what is still open.

Nothing here becomes canonical merely because it is written clearly. Keith must review the decisions, and unresolved source gaps must remain visible.

## Status labels

- **Decided:** strong enough to use as the current design assumption for the package.
- **Provisional:** useful direction supported by the source record, but still needs validation or refinement.
- **Open:** not sufficiently resolved to design around yet.
- **Deferred:** intentionally excluded from the first package version.

## Promotion rule

A working decision may move into canonical material when:

1. it is supported by direct experience, repeated evidence, or a deliberately chosen operating principle;
2. major contradictions have been resolved or documented as situational variants;
3. the instruction is specific enough to use;
4. confidentiality and licensing boundaries are clear; and
5. Keith approves it.

---

# 1. Package purpose and boundary

## D-01: The MQ Package is an operating system, not a retrospective

**Status:** Decided

The MQ Package exists to run a future Gartner Magic Quadrant cycle from end to end. The 2026 retrospective and source record are inputs, not the finished product.

The package must help a coordinator know:

- what stage the program is in;
- what must happen now;
- why it matters;
- who owns each output;
- what the coordinator must retain;
- what can be delegated;
- what signals require escalation;
- what constitutes completion; and
- what must be captured before moving to the next stage.

**Source basis:** The 2026 cycle repeatedly moved to the next stage without converting learning into reusable operating capability.

## D-02: The package serves the vendor-side coordinator first

**Status:** Decided

The primary user is the person coordinating the vendor’s MQ program, especially when that person does not have a mature AR team or inherited operating package.

Other users include:

- the executive sponsor;
- functional executives;
- questionnaire contributors;
- demo owners;
- marketing and sales enablement teams; and
- future coordinators inheriting the program.

The package should explain what each group must do, but it should be organized around the coordinator’s need to run the whole system.

**Source basis:** The coordinator was the only role that needed the complete view, and the absence of a package concentrated memory and judgment in one person.

## D-03: The package covers MQ-specific AR, not all Analyst Relations

**Status:** Decided

The package includes year-round AR work when it directly affects MQ readiness, analyst credibility, evidence, strategy, or evaluation outcomes.

It does not attempt to become a complete AR operating system in its first version.

**Source basis:** The Zone 1 / Zone 2 model shows that MQ depends on year-round AR and company execution, but expanding to all AR work would prevent completion of the MQ Package.

## D-04: The package distinguishes operational truth from public artifacts

**Status:** Decided

The canonical package is the maintained operating core. A book, public playbook, training deck, worksheet, quicksheet, template, or article is an Artifact derived from that core.

Public Artifacts may simplify the system for a specific audience. They should not become competing sources of truth.

**Source basis:** The project was created to prevent scattered files and disconnected outputs from replacing a maintained operating system.

---

# 2. Lifecycle model

## D-05: Use one continuous MQ lifecycle

**Status:** Decided

MQ work is a loop rather than a seasonal project that begins with the Welcome Packet and ends with submission.

The working lifecycle is:

1. **Post-season reset and learning**
2. **Year-round performance and AR management**
3. **Pre-season activation**
4. **Welcome Packet mobilization**
5. **Questionnaire and demo production**
6. **Centralization and submission**
7. **Fact review**
8. **Publication and value capture**
9. Return to post-season

“Return to post-season” is the loop closure, not a separate body of work.

**Source basis:** The 2026 result depended on work before the packet, and the largest process failure was repeatedly moving forward without closing the prior stage.

## D-06: Retain Zone 1 / Zone 2 as an explanatory model

**Status:** Provisional

Use Zone 1 / Zone 2 to explain the relationship between year-round company and AR work and the visible evaluation period:

- **Zone 1:** always-on company execution, evidence creation, analyst relationships, market intelligence, and story continuity.
- **Zone 2:** the bounded evaluation period in which the company packages and proves that work.

The lifecycle stages should remain the operational structure. Zone 1 / Zone 2 should remain a strategic explanation rather than a competing project plan.

**Source basis:** The model clearly explains why an MQ result cannot be manufactured during submission season, but the exact boundary between zones remains fuzzy around pre-season and post-season.

## D-07: Every lifecycle stage needs a gate

**Status:** Decided

Each stage must eventually define:

- entry condition;
- objective;
- required inputs;
- outputs;
- owners;
- coordinator responsibilities;
- executive responsibilities;
- risks and escalation triggers;
- exit criteria; and
- stage retrospective.

The package should not treat a calendar date alone as proof that a stage is complete.

**Source basis:** Work advanced because deadlines arrived, even when setup, documentation, or learning from the prior stage was incomplete.

## D-08: Exact stage names may change without changing the model

**Status:** Provisional

The lifecycle above is stable enough to design against. The final names and whether Questionnaire and Demo become separate playbooks may change after the demo retrospective and first package review.

---

# 3. Nonnegotiable operating principles

## D-09: The underlying result is created before submission season

**Status:** Decided

The package must state clearly that company execution, strategy, product, customer proof, commercial evidence, and analyst credibility create the substance of the evaluation.

MQ-season work improves completeness, coherence, evidence quality, and accuracy. It cannot sustainably manufacture company performance that does not exist.

**Why this matters:** It prevents executives from treating AR as a late-stage messaging function or expecting fact review to repair strategic weaknesses.

## D-10: The coordinator is the structural bottleneck

**Status:** Decided

The package must be designed around the coordinator’s limited judgment and processing capacity.

The coordinator owns or retains:

- whole-submission coherence;
- analyst context and credibility judgment;
- prior-cycle comparison;
- claim calibration;
- cross-functional contradiction resolution;
- final gap analysis; and
- overall timeline and escalation.

The package should aggressively reduce work that does not require that judgment.

**Why this matters:** Coordination, editing, synthesis, and context all accumulated in one role during the 2026 cycle.

## D-11: Functional executives remain accountable for their sections

**Status:** Decided

Executives may delegate drafting, evidence collection, or detailed contribution. They do not delegate accountability for completeness, accuracy, priority, and functional signoff.

The coordinator should be authorized to assign work upward and escalate missing or inadequate contributions.

**Why this matters:** The coordinator cannot personally create company evidence or authoritative functional claims.

## D-12: Optimize for the actual team and risk level

**Status:** Decided

The operating model must reflect:

- size and maturity of the AR team;
- whether the company has a reusable package;
- certainty of inclusion;
- length of the evaluation window;
- stakeholder experience;
- placement or exclusion risk; and
- coordinator capacity.

A company with one coordinator, limited inherited material, and a compressed timeline may need early broad delegation followed by central tightening. It should not copy a low-burden process designed for a mature market leader with a full team.

## D-13: Give contributors imperfect direction early

**Status:** Decided

Question-level or section-level ownership should be assigned as early and specifically as practical. Contributors should be told that assignments are a starting point and that functional owners must scan beyond their tags.

Waiting for perfect decomposition is worse than giving useful but incomplete direction.

**Why this matters:** Under-tagging and weak orientation made the questionnaire more overwhelming and transferred work back to the coordinator.

## D-14: Work returns continuously

**Status:** Decided

Questionnaire answers, demo components, evidence, and review feedback should return as they become ready rather than in one final batch.

The coordinator processes material throughout the cycle while contributors continue working.

**Why this matters:** Continuous flow exposes gaps early and prevents centralization from becoming an impossible end-stage pileup.

## D-15: The coordinator gets protected processing time

**Status:** Decided

The package must include explicit coordinator-only blocks for:

- prior-year comparison;
- contribution processing;
- synthesis;
- contradiction review;
- final editing; and
- submission validation.

These blocks should be treated as project requirements, not personal calendar preferences.

## D-16: The submission environment is the operational source of truth

**Status:** Decided

The live portal or official submission system governs what can actually be submitted. Workbooks, trackers, and offline copies are aids and must be checked against it before work is distributed.

**Why this matters:** The 2026 workbook implied fields that did not exist in the portal, creating wasted effort.

## D-17: Packet Day is scripted

**Status:** Decided

The package must include a prewritten Packet Day plan that eliminates avoidable project-design decisions when the packet arrives.

The plan should cover at least:

- coordinator calendar clearing;
- tiger-team communication;
- schedule conversion;
- workspace setup;
- kickoff scheduling;
- ownership confirmation;
- portal/workbook comparison;
- prior-cycle comparison; and
- analyst-message monitoring.

## D-18: Every important action explains why

**Status:** Decided

Checklists should explain the failure each action prevents, why the timing matters, and what happens if the action is skipped.

**Why this matters:** An unexplained checklist is likely to be ignored under pressure or by the next coordinator.

## D-19: Every stage ends with a written retrospective

**Status:** Decided

A stage does not close until a short retrospective captures:

- intended outcome;
- actual result;
- what helped;
- what broke or surprised the team;
- what changes for the next stage or cycle; and
- what must be added to the package immediately.

The final post-season retrospective aggregates these records instead of reconstructing the cycle from memory.

## D-20: Executive expectation-setting is continuous

**Status:** Decided

The package must include executive communications or scripts at minimum for:

- year-round responsibility;
- pre-season priority and ownership;
- Packet Day mobilization;
- delayed or inadequate contribution escalation;
- pre-fact-review expectations;
- publication pivot; and
- post-season business decisions.

**Why this matters:** The 2026 cycle had insufficient urgency early and excessive expectations of change late.

## D-21: Fact review separates facts from judgment

**Status:** Decided

The fact-review method must classify proposed concerns into at least:

- factual error;
- materially misleading nuance;
- analyst judgment;
- strategic disagreement for the next cycle; and
- internal preference with no valid review action.

The package must prevent fact review from becoming an attempt to rebuild the evaluation.

## D-22: Publication is an operating stage

**Status:** Decided

The evaluation does not create business value merely by being published. The package must cover trigger-ready communication, enablement, campaigns, competitive framing, team recognition, and measurement.

The coordinator must lead a clear shift from correction to leverage.

## D-23: The corporate story must pre-exist the submission

**Status:** Decided

The submission should express the company strategy already being executed and discussed with analysts.

The package should not encourage creation of an isolated MQ narrative that conflicts with roadmap, customer evidence, commercial claims, executive statements, or analyst memory.

## D-24: Every cycle updates the package

**Status:** Decided

The MQ result and the improved operating package are both outputs of the cycle.

Stage retrospectives, analyst feedback, campaign results, missed evidence, changed criteria, and workflow learning should update the package before the program returns to normal operations.

---

# 4. Required package architecture

## D-25: Use one canonical spine with modular stage guidance

**Status:** Provisional

The first canonical package should have one central operating-system document that explains:

- purpose and scope;
- lifecycle;
- roles and governance;
- operating principles;
- how to navigate the package; and
- how the package is maintained.

Detailed stage guidance can then live in modular playbooks or sections without repeating the foundation.

**Reason:** One giant document will be difficult to operate, while disconnected stage files will lose the end-to-end system.

## D-26: Each stage module follows one repeatable template

**Status:** Provisional

Proposed stage-module structure:

1. Purpose
2. When this stage starts
3. Required inputs
4. Outcomes and exit criteria
5. Roles and accountability
6. Coordinator actions
7. Stakeholder actions
8. Executive actions
9. Timeline and cadence
10. Risks and escalation triggers
11. Tools, templates, and scripts
12. Stage retrospective
13. Open variants or situational adjustments

This template should be tested on one stage before being applied to all stages.

## D-27: Reusable tools remain separate from explanatory guidance

**Status:** Provisional

The package should eventually include reusable tools such as:

- lifecycle map;
- pre-season activation plan;
- stakeholder map and RACI;
- setback schedule;
- Packet Day checklist;
- portal/workbook audit;
- prior-cycle comparison worksheet;
- questionnaire assignment tracker;
- demo tracker;
- gap and escalation tracker;
- final submission review checklist;
- fact-review scorecard;
- executive scripts;
- publication sequence;
- campaign and value tracker; and
- stage-retro template.

These should be linked from the canonical method rather than embedded repeatedly.

## D-28: Scripts are first-class operating assets

**Status:** Decided

The package should include language for predictable high-friction moments, not just abstract advice.

Priority scripts:

- executive sponsor setup;
- contributor kickoff;
- assignment and tagging explanation;
- delayed contribution escalation;
- pre-fact-review expectations;
- fact-versus-judgment framing;
- publication pivot;
- team recognition; and
- post-season decision meeting.

**Source basis:** Organizational psychology repeatedly became an operating constraint.

## D-29: Source evidence remains linked, not copied into canonical files

**Status:** Decided

Canonical guidance should link back to the relevant source document or source section when rationale or history matters.

It should not reproduce the entire retrospective, raw notes, or repeated context.

## D-30: Situational variants belong inside the method

**Status:** Provisional

The package should identify when the operating model changes based on team maturity, timeline, inclusion certainty, and program risk.

It should not pretend one workflow is universally optimal.

A likely first variant is:

- **Compressed / coordinator-constrained model:** broad early mobilization, frequent escalation, intense protected synthesis.
- **Mature / well-resourced model:** more pre-mapped ownership, lower coordination burden, more specialized review roles.

This needs validation before becoming canonical.

---

# 5. Decisions by lifecycle stage

## Post-season reset and learning

### D-31: Separate project and business retrospectives

**Status:** Decided

The package should distinguish:

1. **Project retrospective:** how the MQ cycle was run.
2. **Business and product retrospective:** what the result and feedback imply for strategy, product, evidence, positioning, and intentional disagreement.

Combining them risks allowing operational complaints to crowd out strategic implications or vice versa.

### D-32: Capture next-cycle actions twice

**Status:** Provisional

- Capture provisional next-cycle actions immediately after submission while operating details are fresh.
- Formally approve the next-cycle plan after publication and analyst feedback.

This resolves the source conflict between “start next year immediately” and “wait until the evaluation is complete.”

## Year-round performance and AR management

### D-33: Maintain an MQ readiness view year-round

**Status:** Provisional

The package should maintain visibility into:

- known analyst concerns;
- company strategy and narrative;
- product and roadmap evidence;
- customer proof;
- commercial and operational evidence;
- relationship and credibility needs;
- expected criteria changes; and
- gaps requiring cross-functional action.

The exact artifact and cadence remain open.

## Pre-season activation

### D-34: Pre-season is a formal stage

**Status:** Decided

The stage begins before the Welcome Packet and includes context reactivation, prior-cycle review, stakeholder preparation, tool staging, calendar protection, and executive alignment.

### D-35: Exact activation window remains open

**Status:** Open

Candidate windows include four, six, or eight weeks before the expected packet. The package should not lock a duration until the work is estimated and calendar variability is considered.

## Welcome Packet mobilization

### D-36: Day 0, Day 1, and Week 1 must be separated

**Status:** Provisional

The Packet Day checklist should distinguish immediate actions from work that can happen over the first week. This prevents every setup task from appearing equally urgent.

The exact allocation remains to be designed.

## Questionnaire and demo production

### D-37: Questionnaire and demo run in parallel but may need separate playbooks

**Status:** Provisional

They share principles such as ownership, continuous flow, review, escalation, and protected coordinator time.

They involve different work products and expertise. The demo source record is too incomplete to decide whether they should share one module or two.

### D-38: Contributor support uses multiple channels

**Status:** Provisional

The package should likely combine:

- all-stakeholder kickoff;
- written assignments;
- asynchronous guidance;
- office hours; and
- one-on-one support for complex areas.

The exact mix should depend on team size and contributor experience.

## Centralization and submission

### D-39: Centralization is a protected gate

**Status:** Decided

Centralization begins only when expected functional inputs have been returned or explicitly escalated.

The stage must include a defined review sequence and protected coordinator time. It should not be treated as the natural continuation of open contribution drafting.

### D-40: Final signoff structure remains open

**Status:** Open

The package still needs to determine:

- which functional executives sign off;
- what they are approving;
- whether the executive sponsor gives final business signoff;
- how late objections are handled; and
- what remains solely the coordinator’s judgment.

## Fact review

### D-41: Prepare executives before the draft arrives

**Status:** Decided

Expectation-setting should occur roughly before the anticipated draft, not at the first emotionally charged review meeting.

The exact timing can vary. The action cannot be skipped.

### D-42: Use a scorecard and one controlled submission path

**Status:** Provisional

All proposed fact-review changes should be recorded, classified, prioritized, and submitted through a controlled coordinator-owned process.

The scorecard design remains to be created.

## Publication and value capture

### D-43: Prepare trigger-ready materials

**Status:** Decided

Because publication timing can move, core materials should be ready to activate rather than tied to one immovable date.

### D-44: Define value measures before publication

**Status:** Provisional

The package should set intended measures before launch. Candidate measures include:

- sales usage;
- influenced opportunities;
- campaign engagement;
- conversion effects;
- analyst-report downloads;
- competitive use;
- executive and employee amplification; and
- qualitative credibility signals.

The smallest useful measurement set is still open.

---

# 6. Known open decisions

The following should remain visibly unresolved:

1. Exact lifecycle names and final stage boundaries
2. Final Zone 1 / Zone 2 definition
3. Exact pre-season activation window
4. Full demo workflow
5. Whether Questionnaire and Demo use one module or two
6. Customer-reference workflow, where applicable
7. Final review and executive signoff matrix
8. Exact coordinator processing-time model
9. Gap-sweep cadence
10. Office-hours versus one-on-one support model
11. AI uses, controls, and confidentiality boundaries
12. Fact-review scorecard thresholds
13. Publication value measures
14. Year-round readiness artifact and cadence
15. Public, employer-specific, private, and licensed package layers
16. Which tools become public Artifacts first

These open questions should not prevent work on the stable package foundation.

---

# 7. Deferred from version 1

## D-45: Defer a complete AR operating system

**Status:** Deferred

Broader briefing programs, inquiry strategy, analyst segmentation, event strategy, and full market-intelligence operations are out of scope unless directly required by an MQ stage.

## D-46: Defer monetization and packaging decisions

**Status:** Deferred

The first priority is a functioning package. Pricing, fractional-service packaging, course design, gated downloads, and productization should not shape the core method prematurely.

## D-47: Defer polished public narrative

**Status:** Deferred

A public book or playbook should be written after the operating system is coherent and tested. It should not be used to force premature simplicity into the working package.

---

# 8. Recommended build order

## Increment 1: Review and correct this working decision set

Keith reviews:

- whether each “Decided” item is truly decided;
- whether any decision overstates the source record;
- whether important operating principles are missing;
- whether the lifecycle is usable; and
- whether any content should be private or generalized.

## Increment 2: Fill blocking source gaps

Complete only the gaps that block package architecture:

1. focused demo retrospective;
2. publication and immediate post-season update;
3. final review/signoff reconstruction, if recoverable.

Do not delay all package work until every historical detail is available.

## Increment 3: Create the canonical operating-system spine

Proposed file:

`canonical/mq-operating-system.md`

It should include only approved foundation:

- purpose and boundary;
- lifecycle;
- roles and governance;
- nonnegotiable principles;
- package navigation; and
- maintenance rule.

## Increment 4: Build the highest-risk stage modules first

Recommended order:

1. Pre-season activation
2. Welcome Packet mobilization
3. Questionnaire production
4. Centralization and submission
5. Fact review
6. Publication and value capture
7. Post-season reset
8. Year-round management
9. Demo, after source gap is filled

This order addresses the clearest 2026 failures first rather than following chronology mechanically.

## Increment 5: Build shared tools and scripts

Start with:

1. stage-retro template;
2. Packet Day checklist;
3. contributor kickoff script;
4. stakeholder/RACI template;
5. portal/workbook audit;
6. gap and escalation tracker;
7. fact-review scorecard and executive script; and
8. publication pivot sequence.

## Increment 6: Run a consistency review

Check that:

- stage modules use the same lifecycle and terms;
- ownership is not contradictory;
- one task does not have multiple canonical homes;
- every checklist action has a reason;
- open decisions remain labeled;
- sources and licensing boundaries are traceable; and
- the package can be used without reading the 2026 retrospective.

## Increment 7: Derive the first public Artifacts

Choose Artifacts based on standalone user value, not ease of extraction.

Likely early candidates:

- MQ lifecycle map;
- pre-season readiness checklist;
- Packet Day quicksheet;
- stage-retro template;
- fact-review executive guide; and
- public MQ operating playbook.

The Artifact roadmap should be decided only after the canonical spine and first stage modules exist.

---

# 9. Review questions for Keith

1. Is the package primarily for a one-person or small-team coordinator, or should the core method be neutral with variants?
2. Are all items labeled **Decided** actually nonnegotiable?
3. Is the lifecycle correct enough to become the package spine?
4. Does “Post-season reset and learning” belong first in the cycle, or should the operating system begin with year-round management?
5. Should Questionnaire and Demo remain together until the demo retrospective, or separate now?
6. Is “early broad delegation followed by central tightening” the right explicit operating model for the target user?
7. What important lesson from 2026 is missing from the nonnegotiable principles?
8. Which source gaps truly block canonical work?
9. Does the proposed build order match the package you need for the next cycle?
10. Is any decision written too cleanly compared with what the evidence actually supports?

---

# 10. Decision summary

The current working architecture is:

- one continuous MQ lifecycle;
- a vendor-side coordinator as the primary user;
- one canonical operating-system spine;
- modular stage guidance;
- separate reusable tools and scripts;
- early delegation with central synthesis;
- explicit executive accountability;
- protected coordinator judgment time;
- written retrospectives at every gate;
- fact review constrained to facts and material nuance;
- publication treated as value creation; and
- package maintenance as a required output of every cycle.

The next change should come from Keith’s review of these decisions, not from writing the canonical playbook automatically.
