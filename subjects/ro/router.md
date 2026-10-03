# router

**Verdict: could not verify.** Argusic Score 40 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/weave-os/router, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/router

## Pinned environment

- Project commit: `6f4674498ac23dd2a9c2f6da3e9ebe796c27b6c4`
- Test commit: `6f4674498ac23dd2a9c2f6da3e9ebe796c27b6c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 3; wall time 6.3 to 38.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 8 | 6.3 | 2 | 2 | [run](https://argusic.com/run/968e0248-87d5-49d2-999a-048dbf218857) |
| 2 | fail | 50 | 34 | 38.9 | 5 | 5 | [run](https://argusic.com/run/9d2b1fbd-f5ae-452e-9274-934c61a092d0) |
| 3 | fail | 20 | n/a | 13.9 | 0 | 0 | [run](https://argusic.com/run/4cf668b9-7ca3-4d1f-8af0-9c6907be032e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25 not in container; downloaded and installed manually`
- 1 min: `Full app launch requires Postgres (POSTGRES_USER env var) , no Docker available in container, so the server binary panics on startup`

Attempt 2:

- 2 min: `Go 1.25+ not installed`
- 10 min: `Test failure: TestNewTransport_ConfiguresHTTP2Keepalives , Go 1.27+ changed http2.ConfigureTransports to use Protocols/RegisterProtocol instead of TLSNextProto`
- 5 min: `Router needs CGO + ORT tag + ONNX Runtime library + libtokenizers for cluster scorer embedder`
- 3 min: `Router needs Jina v2 model files from HuggingFace for embedder`
- 5 min: `Router needs GCP Pub/Sub emulator (gRPC) for cache invalidation , Java or Docker required`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
