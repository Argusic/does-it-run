# shopee-sdk

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/congminh1254/shopee-sdk, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/shopee-sdk

## Pinned environment

- Project commit: `e35fba777bab34f70a19f57b03d63d7248ced3c8`
- Test commit: `e35fba777bab34f70a19f57b03d63d7248ced3c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7 to 59.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 59.1 | 0 | 0 | [run](https://argusic.com/run/078391ba-9cff-447a-b47b-0e367c3c1400) |
| 2 | pass | 100 | 0.1 | 7 | 1 | 1 | [run](https://argusic.com/run/7cf8b899-cbaa-4e6d-8605-56bce1283d9a) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `globalThis.File is undefined on Node.js 18, causing FileClass is not a constructor in 5 tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
