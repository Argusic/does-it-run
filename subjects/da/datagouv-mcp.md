# datagouv-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/datagouv/datagouv-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/datagouv-mcp

## Pinned environment

- Project commit: `5a37d6f0f1da5504fd12918883498c26d6c28320`
- Test commit: `5a37d6f0f1da5504fd12918883498c26d6c28320`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.6 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 4.6 | 1 | 1 | [run](https://argusic.com/run/bbfc3f87-1610-40a4-87e1-cec54ce43ef3) |
| 2 | pass | 100 | 3 | 8.7 | 1 | 1 | [run](https://argusic.com/run/0d100811-1555-4691-923e-0c6d3f249541) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `requires-python=>=3.13,<3.15 but only Python 3.12 available`

Attempt 2:

- 10 min: `3 tests failed because hardcoded dataset/resource fixture IDs (55e4129788ee386899a46ec1, 3b6b2281-b9d9-4959-ae9d-c2c166dff118) no longer exist on data.gouv.fr API - returned 404`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
