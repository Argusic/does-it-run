# MotionClone

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/blixvip/MotionClone, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/motionclone

## Pinned environment

- Project commit: `30b1e5a271445eddfde143f8f17370c3fca1a7f6`
- Test commit: `30b1e5a271445eddfde143f8f17370c3fca1a7f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7.8 | 8 | 3 | 3 | [run](https://argusic.com/run/02931b86-000a-41db-a96d-ac70b8b44254) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node.js (v18.19.1) too old for HyperFrames (requires 22+)`
- 0.5 min: `sharp native binary missing (optional deps not installed by npm ci)`
- 1.5 min: `Playwright browser launch fails: no Google Chrome installed, channel='chrome' not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
