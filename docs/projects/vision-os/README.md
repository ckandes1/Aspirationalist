# Vision OS

## Charter

**Vision link:** Aspirationalist's mission is to increase momentum toward a better future. Vision OS is the mechanism that converts that stated intent into weekly execution — for Keith first, and eventually as a transferable artifact.

**Active hypothesis:** TODO — Keith to define. The blueprint exists but has never been run against a live project, so there is no bet on the table yet.

**Kill criteria:** TODO — Keith to define. Likely candidate: if two consecutive quarters pass without a project charter surviving its own kill criteria, the framework is theater rather than a system.

**30–90 day scope:** TODO — Keith to define. The obvious first test is charter the MQ Package and run one full weekly reflection loop against it.

**Status:** Canonical framework written, unapplied. No weekly reflection has been run.

## What this project is

Vision OS is the system for translating a long-term vision into daily execution without the middle of that chain going missing.

The problem it solves is the feeling of being directionless while still being busy. That happens when there is a vision and there are daily tasks, but nothing structural in between. Vision OS is that intermediate scaffolding.

The canonical framework lives at:

`canonical/operational-blueprint.md`

## The core idea

Execution is treated as a hypothesis validation engine rather than a project plan.

A vision is mapped to several possible paths. The quickest and most testable one is selected, bound to a 30-to-90 day window, and given explicit criteria that would kill it. If it fails those criteria, it is eliminated rather than carried forward on momentum.

The chain:

**vision → candidate hypotheses → one bet → 30–90 day bound scope → weekly reflection → daily time blocks**

Two constraints do most of the work:

- No more than three active priorities.
- One active hypothesis per priority.

## Relationship to the rest of the repo

Vision OS is a project like any other, but its canonical material governs how other projects are chartered. The `Project Charter` rules in `AGENTS.md` are the applied form of Section 3 of the blueprint.

This means a change to the blueprint is a change to how every project in the repo is structured. Treat edits to `canonical/operational-blueprint.md` as architectural.

## Current state

The blueprint is canonical. Nothing has been run through it.

No project in `docs/projects/` currently carries a charter, including this one. The framework has not yet been tested against real work, which means its weakest claims — that three priorities is the right ceiling, that 30–90 days is the right window, that kill criteria actually get enforced — are untested assumptions rather than findings.

## Next action

Charter the MQ Package. It is the active anchor project and the first honest test of whether the framework survives contact with real work.

## How material matures

`source → working → canonical → artifact`

There is currently no `source/`, `working/`, or `artifacts/` folder. Create them only when the work needs them.

A public artifact version of this framework is plausible — the problem it addresses is common — but it should not be built until the framework has been run against at least one real project and revised from what that produced.
