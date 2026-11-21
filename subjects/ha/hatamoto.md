# hatamoto

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Zen-Labs-Corp/hatamoto, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/hatamoto

## Pinned environment

- Project commit: `7b741ab6020fde4d71b03e93719bea9094b4fb70`
- Test commit: `7b741ab6020fde4d71b03e93719bea9094b4fb70`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 44.2 to 44.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.4 | 44.2 | 1 | 1 | [run](https://argusic.com/run/cc1de1a8-01f6-47b4-b9c4-f3d2286b013f) |

## What was observed on a clean machine

Attempt 1:

- `PostgreSQL not available in container (no docker, no psql)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
