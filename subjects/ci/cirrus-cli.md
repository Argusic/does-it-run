# cirrus-cli

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cirruslabs/cirrus-cli, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/cirrus-cli

## Pinned environment

- Project commit: `1769788a20dc72f6aef85bcdc92abaa1bf061cdc`
- Test commit: `1769788a20dc72f6aef85bcdc92abaa1bf061cdc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 40.3 to 42.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 40.3 | 0 | 0 | [run](https://argusic.com/run/3bc5122c-1396-4ebc-a325-fd937da8158e) |
| 2 | pass with mocks | 92 | 12 | 42.6 | 2 | 2 | [run](https://argusic.com/run/7c7c4a8e-5020-4956-a7c7-f124a34e4f33) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go 1.27+ not available in environment`
- 10 min: `Two tests (TestAdditionalInstanceCredentials, TestValidateCloudInstance) fail because grpc.cirrus-ci.com:443 is unreachable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
