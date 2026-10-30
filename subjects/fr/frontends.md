# frontends

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shopware/frontends, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/frontends

## Pinned environment

- Project commit: `5961f55b9f7cebad626cc073ae0bf857aa26f91b`
- Test commit: `5961f55b9f7cebad626cc073ae0bf857aa26f91b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | n/a | 10 | 2 | 2 | [run](https://argusic.com/run/971f2237-7316-4f10-b79c-e1126014bbee) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 is too old; project requires Node ^22.19.0 || ^24.11.0 || >=26.0.0`
- 1 min: `pnpm not available in the environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
