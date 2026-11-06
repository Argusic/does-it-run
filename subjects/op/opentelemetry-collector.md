# opentelemetry-collector

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-telemetry/opentelemetry-collector, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/opentelemetry-collector

## Pinned environment

- Project commit: `ee42c62804c0d2d225bebdd2b157fd8b0e342de3`
- Test commit: `ee42c62804c0d2d225bebdd2b157fd8b0e342de3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.8 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 10.3 | 1 | 1 | [run](https://argusic.com/run/6985d1a8-6dc8-430b-9791-98ac14f5921e) |
| 2 | pass | 90 | 2 | 9.8 | 2 | 1 | [run](https://argusic.com/run/585078e8-72b9-4598-be14-eeaa5a3f6b91) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go runtime not found in container`

Attempt 2:

- 2 min: `Go runtime not installed in container`
- 1 min: `2 IPv6-related test failures: TestGetAvailableLocalIpv6Address and TestServiceTelemetryZPages/ipv6 fail with 'bind: cannot assign requested address' because container has no IPv6 loopback`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
