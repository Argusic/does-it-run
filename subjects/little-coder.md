# little-coder

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/itayinbarr/little-coder, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/little-coder

## Pinned environment

- Project commit: `a9e467f2be43b78441d723c84f173b98771b51ef`
- Test commit: `a9e467f2be43b78441d723c84f173b98771b51ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.4 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.1 | 6.8 | 3 | 3 | [run](https://argusic.com/run/c7d7e10f-c832-47e7-bf0d-e6fb0166b053) |
| 2 | pass | 100 | 2 | 4.4 | 2 | 2 | [run](https://argusic.com/run/ad5a59f5-e18b-41dc-be81-5bbbaa98b31c) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18.19.1 is insufficient , project requires >=22.19.0`
- 2.5 min: `Playwright browsers not installed , 3 live integration tests failed`
- 1.5 min: `Python PEP 668 prevents global pip install for benchmark tests`

Attempt 2:

- 1 min: `Node.js v18.19.1 is below the required >=22.19.0`
- 1 min: `Playwright browser binaries missing (3 vitest integration tests failed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
