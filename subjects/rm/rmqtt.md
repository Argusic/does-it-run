# rmqtt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rmqtt/rmqtt, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/rmqtt

## Pinned environment

- Project commit: `f57d95ec10d1cd1fddf46693cfd60b2ea2d69315`
- Test commit: `f57d95ec10d1cd1fddf46693cfd60b2ea2d69315`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.8 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 24.8 | 4 | 4 | [run](https://argusic.com/run/70b55c6d-f5b6-4bbd-b3c4-c9ba88c6df5c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `rustc/cargo not found in environment`
- 2 min: `protoc not found, blocking handy-grpc build`
- 1 min: `logger init failed: Permission denied on /var/log/rmqtt`
- `http-api storage init error: Permission denied on /var/log/rmqtt/.cache`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
