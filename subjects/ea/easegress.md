# easegress

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/easegress-io/easegress, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/easegress

## Pinned environment

- Project commit: `3bdb1923a213334fad95dd98ca35dac7dd4c391c`
- Test commit: `3bdb1923a213334fad95dd98ca35dac7dd4c391c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 18.1 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 18.1 | 1 | 1 | [run](https://argusic.com/run/a10b2b5c-3d8a-4414-a606-23a66a8b35dd) |
| 2 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/ae376922-2ac0-4b18-b0e8-e51a60901526) |

## What was observed on a clean machine

Attempt 1:

- `Two tests (TestPostgresClient, TestRedisClientIndexOperations) require Docker via testcontainers-go, which is not available in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
