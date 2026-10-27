# HAProxy-configs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HariSekhon/HAProxy-configs, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/haproxy-configs

## Pinned environment

- Project commit: `df324360a355f2c793c66edce93ee99f4d23978f`
- Test commit: `df324360a355f2c793c66edce93ee99f4d23978f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 8 | 3 | 3 | [run](https://argusic.com/run/e5efc499-3076-4a5c-b655-62fc2ff6c483) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `haproxy binary not found on system`
- 5 min: `check-ssl keyword not recognized in configs (HAProxy built without SSL)`
- 2 min: `bc command not found, preventing HAProxy version check`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
