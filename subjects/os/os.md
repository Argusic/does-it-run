# os

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iblai/os, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/os

## Pinned environment

- Project commit: `4f4b145bbbfea09b3cd51a6e59eeacb16c2a6379`
- Test commit: `4f4b145bbbfea09b3cd51a6e59eeacb16c2a6379`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 12.2 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 14.3 | 0 | 0 | [run](https://argusic.com/run/e27b1e3e-38ae-4e3a-9f27-ee8813872fdb) |
| 2 | pass | 100 | 0.6 | 12.2 | 0 | 0 | [run](https://argusic.com/run/e87f9e27-bc20-4b4d-9d1b-fa19a139ddee) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
