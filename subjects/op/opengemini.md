# openGemini

**Verdict: runs.** Argusic Score 57.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openGemini/openGemini, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/opengemini

## Pinned environment

- Project commit: `7fded2ceaf17f70a0cfbd0f8753837c26b5858c5`
- Test commit: `7fded2ceaf17f70a0cfbd0f8753837c26b5858c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 12.3 to 47.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 12.3 | 0 | 0 | [run](https://argusic.com/run/829388e2-71d8-4706-be0c-3f1798d141bc) |
| 2 | pass | 95 | 47 | 47.8 | 4 | 3 | [run](https://argusic.com/run/bfca6858-6b1a-4a50-be49-9b2b4b495fc1) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `go binary not found in container`
- 1 min: `python3 click module not installed`
- `TestValidateQueryTimeRange fails due to timezone diff (expected CST, got UTC)`
- `app/ts-sql/sql test failures from port conflict with running server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
