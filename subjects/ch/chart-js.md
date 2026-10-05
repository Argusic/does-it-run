# Chart.js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chartjs/Chart.js, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/chart-js

## Pinned environment

- Project commit: `7169e65147a47f3720957a6f156a33c838ab9f57`
- Test commit: `7169e65147a47f3720957a6f156a33c838ab9f57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.5 to 21.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 21.5 | 3 | 3 | [run](https://argusic.com/run/36ceb506-497d-4ed5-a49a-b579885d9905) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not pre-installed; npm install -g pnpm required`
- 3 min: `No Chrome/Firefox browsers installed on system`
- `1 test failure: pixel float tolerance (Expected 33.6 to be close to 31) due to Chromium 157 font rendering differences`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
