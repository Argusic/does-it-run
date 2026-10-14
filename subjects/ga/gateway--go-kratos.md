# gateway

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-kratos/gateway, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/3705e09a-e911-407f-9cfb-8fbf3235f328

## Pinned environment

- Project commit: `a553bef5c1a8cc03ae3d114e5e578c51b8ac06a0`
- Test commit: `a553bef5c1a8cc03ae3d114e5e578c51b8ac06a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 4.9 | 3 | 3 | [run](https://argusic.com/run/3705e09a-e911-407f-9cfb-8fbf3235f328) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `go binary not installed in container`
- `tracing middleware in sample config logs connection-refused noise for localhost:4318 (no OTLP collector)`
- `HTTP-to-gRPC transcoder path not end-to-end verified (no gRPC backend for 127.0.0.1:9000)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
