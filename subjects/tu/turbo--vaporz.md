# turbo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vaporz/turbo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/afef2e63-cbf5-4800-a447-d910fdfc7e79

## Pinned environment

- Project commit: `8088e6bf86ef08edb211e0750eddb6ca7c0b79f4`
- Test commit: `8088e6bf86ef08edb211e0750eddb6ca7c0b79f4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.4 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.5 | 15.4 | 5 | 5 | [run](https://argusic.com/run/afef2e63-cbf5-4800-a447-d910fdfc7e79) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container (required go >= 1.27.1)`
- 1.5 min: `protoc not found (needed for gRPC code generation)`
- 1.5 min: `protoc-gen-go not found (needed for --go_out=plugins=grpc)`
- 1 min: `protoc-gen-buildfields not found (Turbo's own protoc plugin)`
- 2.5 min: `thrift compiler binary not available (TestCreateThriftService integration test fails)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
