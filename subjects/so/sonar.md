# sonar

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/raskrebs/sonar, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/sonar

## Pinned environment

- Project commit: `9c963b8447d6ca08dd4a3c0bc6c0bf27527cd793`
- Test commit: `9c963b8447d6ca08dd4a3c0bc6c0bf27527cd793`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 10.1 | 3 | 3 | [run](https://argusic.com/run/91a4efe8-c478-4ae9-bd91-0e8dff8144f1) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `go not found on PATH`
- 0.8 min: `ss (iproute2) not installed, tests fail with 'exec: ss: not found'`
- `TestAnExitIsKeptWithWhereTheRunCameFrom flaky failure in groupstart`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
