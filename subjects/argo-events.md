# argo-events

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/argoproj/argo-events, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/argo-events

## Pinned environment

- Project commit: `52ed46109a1df5e57d19f0ea3919c63d9617a2d8`
- Test commit: `52ed46109a1df5e57d19f0ea3919c63d9617a2d8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 11.7 | 1 | 1 | [run](https://argusic.com/run/b9bf52a8-dc47-4f01-9487-dfe8ab75d5d9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Go compiler in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
