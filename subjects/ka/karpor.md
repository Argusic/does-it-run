# karpor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KusionStack/karpor, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/karpor

## Pinned environment

- Project commit: `7ac7c795ff47210da7ce3a71b2a28b4e0fba03e1`
- Test commit: `7ac7c795ff47210da7ce3a71b2a28b4e0fba03e1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 20.7 to 20.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 20.7 | 4 | 4 | [run](https://argusic.com/run/2320a1fe-86db-4865-ac92-6396f336738c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed`
- 3 min: `etcd not available for persistence backend`
- 1 min: `Service account signing key file required but not provided`
- 6 min: `Only Elasticsearch search storage type supported , none configured, server refused to start`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
