# ai-avatar-system

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PunithVT/ai-avatar-system, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-avatar-system

## Pinned environment

- Project commit: `0dee976c229b2b6d274f8d04784d7e5be964d7b6`
- Test commit: `0dee976c229b2b6d274f8d04784d7e5be964d7b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.4 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.4 | 1 | 1 | [run](https://argusic.com/run/5ed04f2b-136b-4c2b-b7e5-23e9503b26db) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rate limiter middleware crashes with IndexError when Authorization header contains a bare JWT without 'Bearer ' prefix. This affects every authenticated endpoint called by clients that copy the raw token from the login response.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
