# agav

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/prapaa-ai/agav, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agav

## Pinned environment

- Project commit: `989687b1ac50bcdde8076ad36b4faf32e4570f5e`
- Test commit: `989687b1ac50bcdde8076ad36b4faf32e4570f5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 10.8 | 4 | 4 | [run](https://argusic.com/run/c5ccf06d-7830-4447-972b-43ac4c7adcb6) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 present but project requires >=22.13.0`
- 0.3 min: `pnpm not available with stock Node 22 (corepack key verification failed)`
- 10 min: `Test suite: 55 tests failed out of 6776 (0.8%) in full parallel run , all are timeout/race-condition failures from resource contention`
- 5 min: `Background-jobs coordinator tests 2/2 fail individually due to beforeEach hook timeout (10s) on linux , createCoordinator hangs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
