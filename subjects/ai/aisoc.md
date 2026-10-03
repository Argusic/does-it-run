# AiSOC

**Verdict: runs with mocks.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/beenuar/AiSOC, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/aisoc

## Pinned environment

- Project commit: `f0e8fec9db8ebe56751bc9ddcd7d0bb997a7e8af`
- Test commit: `f0e8fec9db8ebe56751bc9ddcd7d0bb997a7e8af`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.2 to 11.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 28 | 11.2 | 5 | 4 | [run](https://argusic.com/run/c44bcbde-de75-4924-af72-ce4010c9664f) |

## What was observed on a clean machine

Attempt 1:

- `Docker is not installed (no root access) - cannot run make up / make smoke / full stack`
- `Node.js v18.19.1 below >=20.0.0 requirement - vitest test runner fails for TS packages (aisoc-lite, report-card, sdk-ts)`
- 2 min: `Python PEP 668 blocks system-wide pip install - needed venv workaround`
- 1 min: `pnpm not pre-installed (npm -g install needed)`
- `aisoc-ueba service hatchling metadata generation fails (missing packages directive)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
