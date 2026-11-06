# backend

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/prod-forge/backend, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/backend

## Pinned environment

- Project commit: `9e3cb4a660074465ced049e5b8d1c010068dd41a`
- Test commit: `9e3cb4a660074465ced049e5b8d1c010068dd41a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.5 to 21.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 19 | 21.5 | 3 | 2 | [run](https://argusic.com/run/b464a647-7060-41d7-83d0-264adc1352a5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 too old (requires 24+); Prisma 7.10.1 blocked install`
- 6 min: `No Docker, PostgreSQL, or Redis available in container`
- 3 min: `E2E tests (testcontainers) cannot run without Docker daemon`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
