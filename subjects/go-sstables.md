# go-sstables

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thomasjungblut/go-sstables, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/go-sstables

## Pinned environment

- Project commit: `e6e569d469503031064ef1a5e53f7058ecae9528`
- Test commit: `e6e569d469503031064ef1a5e53f7058ecae9528`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.7 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.7 | 2 | 2 | [run](https://argusic.com/run/f88ea790-af8e-4e65-91e2-b0364e408800) |
| 2 | pass | 100 | 0.3 | 2.9 | 0 | 0 | [run](https://argusic.com/run/a5511372-8745-45b7-9ce7-45b0bc7ff40a) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go 1.25 was not installed in the environment`
- 0.1 min: `GOPATH and GOMODCACHE environment variables were unset`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
