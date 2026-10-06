# workbuddy2api-panel

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linguo2625469/workbuddy2api-panel, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/workbuddy2api-panel

## Pinned environment

- Project commit: `1e23c2b27becc43bb74dfc2101a5fbf9867d6963`
- Test commit: `1e23c2b27becc43bb74dfc2101a5fbf9867d6963`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.1 to 27.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 26 | 27.1 | 2 | 2 | [run](https://argusic.com/run/3727641b-48d7-45c1-a69b-78cd22c062b8) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `V compiler does not support .go extension (golang backend removed)`
- 5 min: `Real CodeBuddy OAuth credentials required for upstream API calls`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
