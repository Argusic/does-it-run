# kilo

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/squat/kilo, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kilo

## Pinned environment

- Project commit: `0f78bc1f281fbcb2f542106ba44a29f19eda1349`
- Test commit: `0f78bc1f281fbcb2f542106ba44a29f19eda1349`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30.7 to 30.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 24 | 30.7 | 1 | 1 | [run](https://argusic.com/run/7abc9f4d-0676-4fd7-96e5-02acd5ace6ed) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container (no apt install permission)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
