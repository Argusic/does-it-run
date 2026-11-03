# node-red

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/node-red/node-red, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/node-red

## Pinned environment

- Project commit: `1e85f1efbc8875ad960400905038154a4e4dd76e`
- Test commit: `1e85f1efbc8875ad960400905038154a4e4dd76e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.2 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 43.2 | 6.2 | 2 | 1 | [run](https://argusic.com/run/9b0613c8-00a6-48d5-8e08-b45451f15681) |
| 2 | pass | 100 | 16 | 17.1 | 2 | 2 | [run](https://argusic.com/run/dd56d4c6-550b-48c3-9e08-9eb84fe142e4) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Node.js v18.19.1 does not meet project requirement of >=22.9`
- 5 min: `ssh-keygen not available in container, causing 5 SSH project test failures`

Attempt 2:

- 2 min: `Node.js v18.19.1 not supported (requires >=22.9.0) - red.js and lib/red.js exit with error`
- 5 min: `ssh-keygen not found in container (5 test failures)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
