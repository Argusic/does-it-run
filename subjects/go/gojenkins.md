# gojenkins

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bndr/gojenkins, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gojenkins

## Pinned environment

- Project commit: `b53358041d6023d4cc7bfff8e26e9e3228e0b45b`
- Test commit: `b53358041d6023d4cc7bfff8e26e9e3228e0b45b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.9 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 4.9 | 0 | 0 | [run](https://argusic.com/run/74282f05-c4dc-4f36-8b23-1da98e661146) |
| 2 | pass with mocks | 92 | 5 | 5.4 | 1 | 1 | [run](https://argusic.com/run/3972c1a6-678a-44d2-9453-1f3339ecb0f1) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go compiler (golang) not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
