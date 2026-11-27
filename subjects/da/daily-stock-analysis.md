# daily_stock_analysis

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ZhuLinsen/daily_stock_analysis, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/daily-stock-analysis

## Pinned environment

- Project commit: `be148f39ce3be8bc7f9c2d5b0ad77cd31655e78f`
- Test commit: `be148f39ce3be8bc7f9c2d5b0ad77cd31655e78f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 39 to 39 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 3.5 | 39 | 2 | 0 | [run](https://argusic.com/run/7baf3a9a-5128-46c4-a869-99120704b301) |

## What was observed on a clean machine

Attempt 1:

- `test_fundamental_adapter_contracts: 3 failures due to akshare 1.20.45 API rename (stock_sector_fund_flow_rank -> stock_fund_flow_sector_rank_em) - pre-existing upstream breakage`
- `Web frontend (apps/dsa-web) requires Node >=20.19, only Node 18.19 available - npm ci/lint/build skipped`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
