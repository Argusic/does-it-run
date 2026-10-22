# voxelize

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/voxelize/voxelize, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/voxelize

## Pinned environment

- Project commit: `b5097e45acba0b5e4c457eb7c4294a6797b2b485`
- Test commit: `b5097e45acba0b5e4c457eb7c4294a6797b2b485`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.7 to 26.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 26.7 | 3 | 3 | [run](https://argusic.com/run/d9e29504-dcc5-4d6c-ad8e-95c4f3a953a3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `frame-budget.test.ts: performance.now is read-only in Node 18 (11 tests failed)`
- 2 min: `vitest picked up scripts/engine-boundary/check.test.mjs as a test suite but it uses Node native test runner`
- 1 min: `geology_cost_smoke test: p95 geo chunk cost 538781us blew smoke bound in constrained environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
