# liftbridge

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liftbridge-io/liftbridge, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/liftbridge

## Pinned environment

- Project commit: `af2a662695ce67c099e56d24444afb15bd8df232`
- Test commit: `af2a662695ce67c099e56d24444afb15bd8df232`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 12.1 to 20.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 22 | 20.7 | 2 | 2 | [run](https://argusic.com/run/69e7db86-1184-4474-9dd3-a3c9ce4f5bac) |
| 2 | pass with mocks | 92 | 12 | 12.1 | 4 | 4 | [run](https://argusic.com/run/709bcec3-acdd-43bc-906b-e094ae80ce91) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Go compiler found on system`
- 5 min: `Go 1.27.1 build: undefined http2.TrailerPrefix in grpc v1.79.3 (golang.org/x/net/http2 excluded by go1.27+ build tag)`

Attempt 2:

- 2 min: `go command not found in container`
- `nats-server binary not available (no apt/sudo)`
- 5 min: `Build error: 'http2.TrailerPrefix' undefined in grpc handler_server.go on Go 1.27`
- `server_test.go integration tests fail silently (TestActivityStreamCreateStream hangs/timeouts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
