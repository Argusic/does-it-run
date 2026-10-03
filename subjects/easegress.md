# easegress

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/easegress-io/easegress, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/easegress

## Pinned environment

- Project commit: `3bdb1923a213334fad95dd98ca35dac7dd4c391c`
- Test commit: `3bdb1923a213334fad95dd98ca35dac7dd4c391c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.1 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 18.1 | 1 | 1 | [run](https://argusic.com/run/a10b2b5c-3d8a-4414-a606-23a66a8b35dd) |

## What was observed on a clean machine

Attempt 1:

- `Two tests (TestPostgresClient, TestRedisClientIndexOperations) require Docker via testcontainers-go, which is not available in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
