# temporal

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/temporalio/temporal, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/temporal

## Pinned environment

- Project commit: `d8f9c6d86b2cd0ea5c27d0694a598da84c6d337d`
- Test commit: `d8f9c6d86b2cd0ea5c27d0694a598da84c6d337d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.1 to 54.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28.2 | 54.6 | 4 | 4 | [run](https://argusic.com/run/db3ff869-3dbc-4db3-b7a1-e4979d629b00) |
| 2 | pass | 86.67 | 7 | 11.1 | 3 | 1 | [run](https://argusic.com/run/535fc2f5-522b-4a3e-8170-b49cf06e557c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.0 not installed in container`
- 5 min: `Makefile unit-test target fails: -race flag requires cgo, but Makefile defaults CGO_ENABLED=0`
- 1 min: `make lint-code-fast requires main branch for diff base`
- 8 min: `Some test suites (ScaleManagerSuite, MatchingEngine, TaskQueuePartitionManager) hang when run together in ./service/matching/`

Attempt 2:

- 2 min: `Go 1.27.3 not installed`
- `make lint-code-fast requires main branch ref (detached HEAD)`
- `3 pre-existing flaky matching-engine unit tests fail on backlog timing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
