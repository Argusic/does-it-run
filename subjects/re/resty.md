# resty

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-resty/resty, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/resty

## Pinned environment

- Project commit: `3da7d0987ff4ba931fe55ce8a7f71cb4193fd971`
- Test commit: `3da7d0987ff4ba931fe55ce8a7f71cb4193fd971`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.9 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5.3 | 1 | 1 | [run](https://argusic.com/run/266f1a50-0265-46f5-b9cb-a9e48602dc71) |
| 2 | pass | 100 | 4 | 3.9 | 1 | 1 | [run](https://argusic.com/run/c6329fb9-cd44-45ed-8827-2ec81812e24d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go binary not found in PATH`

Attempt 2:

- 4 min: `no Go toolchain in container: 'go: not found'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
