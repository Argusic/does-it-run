# blades

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-kratos/blades, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/blades

## Pinned environment

- Project commit: `b78fec59029d11e02c135ea10da8986ed006521f`
- Test commit: `b78fec59029d11e02c135ea10da8986ed006521f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.9 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 16.9 | 2 | 2 | [run](https://argusic.com/run/6bab584d-f73b-4e71-bc94-26ae2b5a7c3c) |

## What was observed on a clean machine

Attempt 1:

- 9 min: `go: command not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
