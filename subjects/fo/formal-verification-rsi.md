# Formal-Verification-RSI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sahibzada-allahyar/Formal-Verification-RSI, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/formal-verification-rsi

## Pinned environment

- Project commit: `177a62d5847d4d3b162c53e854a71886bf463de1`
- Test commit: `177a62d5847d4d3b162c53e854a71886bf463de1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 80.6 to 80.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 80.6 | 1 | 1 | [run](https://argusic.com/run/db541974-6a37-4b73-ae4a-872854ba6684) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Test Agent snapshot manifests had temp paths instead of /app, causing all 4 snapshot-integrity tests to fail with 0 graded files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
