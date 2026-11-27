# dapr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dapr/dapr, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/dapr

## Pinned environment

- Project commit: `6801e6d54e908e0f7625e2a467d40359c3eb77d6`
- Test commit: `6801e6d54e908e0f7625e2a467d40359c3eb77d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.4 to 39.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 39.4 | 1 | 1 | [run](https://argusic.com/run/7a5a3c18-5ebd-4056-9c6a-7a2c312596a1) |

## What was observed on a clean machine

Attempt 1:

- `IPv6 loopback not available: Integration test TestIntegration_ReconnectAfterServerRestart fails to bind to [::1]:38887 in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
