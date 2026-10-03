# ECC

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/affaan-m/ECC, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ecc

## Pinned environment

- Project commit: `e482e579415fde18357cafce70f177ae19fd7f03`
- Test commit: `e482e579415fde18357cafce70f177ae19fd7f03`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.1 | 24 | 3 | 0 | [run](https://argusic.com/run/c9096a52-8273-4fc4-a2c8-c07c4383ff52) |

## What was observed on a clean machine

Attempt 1:

- `tests/integration/plan-canvas-e2e.test.js: 9 failed , requires running plan canvas server and browser`
- `tests/integration/hooks.test.js: hangs indefinitely`
- `tests/lib/terminal-spinner.test.js: 1 failed , flaky spinner frame ordering race`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
