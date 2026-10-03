# arcadedb

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ArcadeData/arcadedb, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/arcadedb

## Pinned environment

- Project commit: `9010582b796146c5ded2f273053ddcbf85f9e3d6`
- Test commit: `9010582b796146c5ded2f273053ddcbf85f9e3d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 70.5 to 85.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 85.2 | 3 | 3 | [run](https://argusic.com/run/423a65fc-edd4-4a84-9b5b-ae07b49a4f5a) |
| 2 | fail | 20 | n/a | 70.5 | 0 | 0 | [run](https://argusic.com/run/bdefedd8-3847-4424-a187-47dd99f9201b) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `No Java or Maven installed in the container`
- 2 min: `TimeoutStepTest.shouldWorkWithVeryShortTimeout fails - WorkGuard throws a different TimeoutException message format than the test expects`
- 0.5 min: `Issue6216AlgoWorkKnobBoundsTest.randomWalkHonoursTheCommandTimeoutEvenWithTheWalkMemoryBudgetDisabled fails - OOM during large batch test run when memory is constrained across 14624 concurrent tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
