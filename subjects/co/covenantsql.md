# CovenantSQL

**Verdict: runs with mocks.** Argusic Score 77 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CovenantSQL/CovenantSQL, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/covenantsql

## Pinned environment

- Project commit: `fdaa8a4b909fabcf7023951abebaf4a0203bc24b`
- Test commit: `fdaa8a4b909fabcf7023951abebaf4a0203bc24b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.2 to 11.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 77 | 12 | 11.2 | 4 | 1 | [run](https://argusic.com/run/223bfdcd-c83a-4614-88b4-50f0e247486d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `route/ipv6seed_test.go: TestGenTestNetDomain/TestIPv6Seed fail due to external DNS resolution (bp00.testnet.gridb.io etc.) not available in container`
- 1 min: `proto/proto_test.go: TestEnvelope_GetSet uses goconvey ShouldEqual on context.Context values, which renders as equal but ShouldEqual fails on interface comparison`
- 1 min: `api/service_test.go: TestJSONRPCService websocket server starts in goroutine but test connects before server is ready (timing race)`
- 3 min: `cql-minerd build requires libicu-dev for sqlite_icu tag; built without that tag`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
