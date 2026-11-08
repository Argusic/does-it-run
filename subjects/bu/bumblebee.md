# bumblebee

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/perplexityai/bumblebee, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/bumblebee

## Pinned environment

- Project commit: `8ef7fbce5748ac42d519900950a7de4eb3ec1ad8`
- Test commit: `8ef7fbce5748ac42d519900950a7de4eb3ec1ad8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.7 to 3.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.6 | 0 | 0 | [run](https://argusic.com/run/6d919816-4b05-49a8-a351-ef2aadc9462c) |
| 2 | pass | 100 | 4 | 1.7 | 1 | 1 | [run](https://argusic.com/run/08faa978-3d89-4819-8e1d-3dcbb52e153b) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go 1.25+ not present in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
