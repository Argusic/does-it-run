# graphologue

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/foundation-interface/graphologue, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/graphologue

## Pinned environment

- Project commit: `5c3563203c1afe0bf80a117a463244f2c6ade4d9`
- Test commit: `5c3563203c1afe0bf80a117a463244f2c6ade4d9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 3.7 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1 | 3.7 | 0 | 0 | [run](https://argusic.com/run/55a64677-d2f8-4e63-8d09-3e681df8c6be) |
| 2 | pass with mocks | 92 | 2 | 13.6 | 2 | 2 | [run](https://argusic.com/run/c7baf43f-2c6c-405b-9eb8-59709a24d0b1) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `No browser (Chrome/Chromium/Firefox) installed in container; puppeteer could not install one (Node v18, incompatible puppeteer@25 browsers install helper, and no root for apt)`
- 1 min: `No test files in the repository (react-scripts test: No tests found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
