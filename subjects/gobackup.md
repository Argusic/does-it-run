# gobackup

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gobackup/gobackup, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gobackup

## Pinned environment

- Project commit: `33048dc9b59648c02f6f95989f4d4416007c8c4d`
- Test commit: `33048dc9b59648c02f6f95989f4d4416007c8c4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 6.5 | 2 | 2 | [run](https://argusic.com/run/d13c7aef-1c95-446d-80dd-1bfa10d586b0) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Go compiler (golang) not installed in container`
- 2 min: `Web frontend must be built before Go build (//go:embed dist directive)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
