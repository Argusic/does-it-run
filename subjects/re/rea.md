# rea

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/morluto/rea, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/rea

## Pinned environment

- Project commit: `2160d4fae581243990e539a9c401d1b8824e1763`
- Test commit: `2160d4fae581243990e539a9c401d1b8824e1763`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.4 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 8.1 | 0 | 0 | [run](https://argusic.com/run/d37f8d5d-85f7-429c-81a3-3d3ef28785c5) |
| 2 | pass with mocks | 92 | 30 | 7.4 | 1 | 1 | [run](https://argusic.com/run/64c0a843-f7f1-419b-b85e-be7dd26ce8c7) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Node.js 18.19.1 is installed but project requires ^22.19.0 || >=24.11.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
