# reactivesearch-api

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/appbaseio/reactivesearch-api, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/reactivesearch-api

## Pinned environment

- Project commit: `8d9acac8b4c0f24b86f6c91bc44e4f8bba157b7b`
- Test commit: `8d9acac8b4c0f24b86f6c91bc44e4f8bba157b7b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.8 to 16.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 16.8 | 4 | 4 | [run](https://argusic.com/run/fca308b3-9c24-4b90-a870-0d09bc469930) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go (Golang) not pre-installed in the container`
- 1 min: `Initial build with Tier=test failed - 'invalid plan encountered: test'`
- 3 min: `Pipeline plugin requires Elasticsearch; server fails without ES_CLUSTER_URL`
- `Rules plugin test (TestRunScript) has a pre-existing test failure unrelated to install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
