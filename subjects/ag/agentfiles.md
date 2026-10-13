# agentfiles

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Railly/agentfiles, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agentfiles

## Pinned environment

- Project commit: `b2627e84b4c512430759f55c8d7ac5b54bc368b3`
- Test commit: `b2627e84b4c512430759f55c8d7ac5b54bc368b3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 4.8 | 2 | 2 | [run](https://argusic.com/run/6d2ce1d2-928c-445e-90a2-55d20ac6cf0e) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `bun: not found in container and installer requires unzip (not installed, no root)`
- 6 min: `bun audit failed: 14 vulnerabilities (8 high, 6 moderate) blocking 'bun run check'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
