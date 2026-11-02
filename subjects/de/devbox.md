# devbox

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rudderlabs/devbox, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/devbox

## Pinned environment

- Project commit: `fc2b4270eb803404281e352bb79394a54d28c723`
- Test commit: `fc2b4270eb803404281e352bb79394a54d28c723`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 8.2 | 1 | 1 | [run](https://argusic.com/run/c11b31ef-d3b9-4b56-a3b5-39706a76f6d1) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `8 control-plane tests fail: no PostgreSQL 18 database available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
