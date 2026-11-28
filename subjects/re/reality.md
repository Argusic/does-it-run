# reality

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/howmp/reality, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/reality

## Pinned environment

- Project commit: `0bacb7fce48d981f9ca82be556242375e72db330`
- Test commit: `0bacb7fce48d981f9ca82be556242375e72db330`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 2.5 | 6.6 | 1 | 0 | [run](https://argusic.com/run/ac78baf9-c509-4b65-8e62-62959859c978) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `TestRealityHandshake_Huawei integration test times out when performing REALITY handshake to www.huawei.com:443 from this container environment - client connection hangs indefinitely`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
