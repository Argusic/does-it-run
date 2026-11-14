# finvizfinance

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lit26/finvizfinance, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/finvizfinance

## Pinned environment

- Project commit: `44ded722ae9d3d80328832f4003f437754d29817`
- Test commit: `44ded722ae9d3d80328832f4003f437754d29817`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.3 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.2 | 2.3 | 0 | 0 | [run](https://argusic.com/run/493ca75a-eae9-472a-8fdb-ffd0f7d85614) |
| 2 | pass | 100 | 14 | 12.9 | 4 | 4 | [run](https://argusic.com/run/c96e5475-a4c9-4bf0-b698-8fc559021673) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip install failed (externally-managed-environment on system python)`
- 7 min: `crypto, forex, future, calendar Drift (finviz site migrated to SPA)`
- 3 min: `screener/earnings Drift - cannot fix fully`
- 2 min: `test fixtures outdated for new JSON format`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
