# dynamodump

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bchew/dynamodump, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/dynamodump

## Pinned environment

- Project commit: `58754125a1348fdb7801f746bece147ec0e8cd21`
- Test commit: `58754125a1348fdb7801f746bece147ec0e8cd21`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 17.8 | 8 | 8 | [run](https://argusic.com/run/412d0f85-93e0-4fd4-9674-f53bbda01dca) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install failed due to externally-managed-environment`
- 2 min: `Docker not available for DynamoDB Local`
- 1 min: `moto server requires flask (ModuleNotFoundError: flask)`
- 1 min: `moto server requires flask-cors (ModuleNotFoundError: flask_cors)`
- 1 min: `moto_server CLI does not accept service name as positional arg`
- 1 min: `moto returns KeyError on region name local`
- `test_schema fails: TableSizeBytes 28 != 0 (moto reports 0)`
- `empty/wildcard restore fails: GlobalSecondaryIndexes empty list rejected by DynamoDB`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
