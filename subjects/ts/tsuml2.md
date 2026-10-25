# TsUML2

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/demike/TsUML2, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tsuml2

## Pinned environment

- Project commit: `f4a7e5489b215635447421f0c58bb07ea18c93ad`
- Test commit: `f4a7e5489b215635447421f0c58bb07ea18c93ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.2 to 1.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.15 | 1.2 | 1 | 1 | [run](https://argusic.com/run/2fc343cc-2f09-4cee-bb2e-b97300763c88) |

## What was observed on a clean machine

Attempt 1:

- 0.07 min: `vitest 4.x requires Node >=20; container has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
