# res

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alextnetto/res, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/res

## Pinned environment

- Project commit: `1d05d9c4a9f96d3cd94e9fa49609f98d7e4b4563`
- Test commit: `1d05d9c4a9f96d3cd94e9fa49609f98d7e4b4563`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8.1 | 3 | 3 | [run](https://argusic.com/run/e15ec961-0ae2-48ba-a93a-f03a889766f4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node.js is v18 but project requires >=22 (Playwright needs >=20)`
- 3 min: `Playwright browsers not installed (chromium was missing)`
- 2 min: `Node.js v22.0.0 has a test runner bug where before() hooks don't await async operations before tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
