# Whale

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/usewhale/Whale, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/whale

## Pinned environment

- Project commit: `676a0a228882c457ff4dc00d9d285d972aea4a43`
- Test commit: `676a0a228882c457ff4dc00d9d285d972aea4a43`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 3 | 1 | 1 | [run](https://argusic.com/run/228d7ab2-a48e-47c1-9f5b-9376aa286fa9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
