# cftunnel

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qingchencloud/cftunnel, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/cftunnel

## Pinned environment

- Project commit: `9654f3c0820aef04bd07a9deb9592d9567bfd5c2`
- Test commit: `9654f3c0820aef04bd07a9deb9592d9567bfd5c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.8 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 12.8 | 1 | 1 | [run](https://argusic.com/run/b7b5c14f-f1a1-4843-ac9f-4175e189ae32) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not pre-installed in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
