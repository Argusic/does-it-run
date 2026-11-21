# taskq

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vmihailenco/taskq, licensed BSD-2-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/taskq

## Pinned environment

- Project commit: `ccd27a03f11b65602cbb32d3923a9618f8b4cad9`
- Test commit: `ccd27a03f11b65602cbb32d3923a9618f8b4cad9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13.6 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 18.6 | 2 | 2 | [run](https://argusic.com/run/653db49d-f905-4692-bd6b-c58da93b41f5) |
| 2 | pass | 100 | 2 | 13.6 | 0 | 0 | [run](https://argusic.com/run/8d2e1b78-82c7-4518-9c45-2297b5c14bde) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Go compiler not installed in the container`
- 7 min: `Redis server not running for redisq tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
