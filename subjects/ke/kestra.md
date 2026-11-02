# kestra

**Verdict: runs.** Argusic Score 93.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kestra-io/kestra, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/kestra

## Pinned environment

- Project commit: `4b9c7a1e28eb882562d464df33c93b40fde1d045`
- Test commit: `4b9c7a1e28eb882562d464df33c93b40fde1d045`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 54.6 to 74.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 54 | 54.6 | 4 | 3 | [run](https://argusic.com/run/5c0124f8-9cad-40d1-8763-e71c6b641f11) |
| 2 | pass | 100 | 92 | 74.6 | 5 | 5 | [run](https://argusic.com/run/a3347c0e-9fd4-4e8b-b5a9-f33f0a4d2664) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `JDK 25 not found in environment`
- 3 min: `sub.localhost DNS resolution fails in container, causing HttpClientAllowedListWildcardTest to throw RuntimeException instead of HttpClientRequestException`
- `HttpClientTest uses Testcontainers (Docker), which is not available in this container`
- 3 min: `Node.js 18 is too old for UI (requires >=24), npm 9 is too old (requires >=11.7)`

Attempt 2:

- 2 min: `JDK 25 not pre-installed in container`
- 2 min: `Node.js v18 too old (requires >=24)`
- `Testcontainers-based HttpClientTest requires Docker (not available)`
- 1 min: `Playwright browser not found for storybook tests`
- `ExecutionServiceTest.replayEachSeq failed due to timing in parallel run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
