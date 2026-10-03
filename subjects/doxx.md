# doxx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bgreenwell/doxx, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/doxx

## Pinned environment

- Project commit: `062819a10f423f2b2ce52be6d264e9069b1b9a40`
- Test commit: `062819a10f423f2b2ce52be6d264e9069b1b9a40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.2 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 9.2 | 1 | 1 | [run](https://argusic.com/run/6ed57a12-4666-47a1-9c83-2227ec3e2aaf) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `NO_COLOR=1 env var causes crossterm 0.28 to suppress all ANSI color output in tests, causing 2 test failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
