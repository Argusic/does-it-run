# MyPerf4J

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LinShunKang/MyPerf4J, licensed BSD-3-Clause, written in Java.

Evidence and recordings: https://argusic.com/subject/myperf4j

## Pinned environment

- Project commit: `9846842704821d26ce1f44fd5896b654ae4d326f`
- Test commit: `9846842704821d26ce1f44fd5896b654ae4d326f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 17.8 to 21 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 21 | 2 | 2 | [run](https://argusic.com/run/65370bd9-3022-4cd7-8bcc-cbf9e7f95163) |
| 2 | pass with mocks | 92 | 16 | 17.8 | 2 | 2 | [run](https://argusic.com/run/9a43b8dd-519c-4d2c-91e2-fe828a7308fc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ILoggerTest.test: IllegalState: MyProperties is not initial yet!!!`
- 5 min: `InfluxDbV2ClientTest fails AssertionError: needs running InfluxDB v2 server on port 8086 for REST API calls`

Attempt 2:

- 3 min: `ILoggerTest fails with "MyProperties is not initial yet!!!" because it does not initialize MyProperties before calling loadMetricsConfig()`
- 2 min: `InfluxDbV2ClientTest fails because it tries to connect to a real InfluxDB instance at 127.0.0.1:8086 which is not running`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
