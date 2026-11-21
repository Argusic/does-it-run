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
- Valid runs: 2; wall time 20 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 24.8 | 4 | 4 | [run](https://argusic.com/run/70b55c6d-f5b6-4bbd-b3c4-c9ba88c6df5c) |
| 2 | pass | 100 | 9 | 20 | 4 | 4 | [run](https://argusic.com/run/d5e9deb3-b93a-4602-a9a1-2f360e2890a3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `rustc/cargo not found in environment`
- 2 min: `protoc not found, blocking handy-grpc build`
- 1 min: `logger init failed: Permission denied on /var/log/rmqtt`
- `http-api storage init error: Permission denied on /var/log/rmqtt/.cache`

Attempt 2:

- 1 min: `protoc (protobuf compiler) was not pre-installed, required by handy-grpc and pulsar build scripts`
- 1 min: `Rust toolchain not pre-installed`
- 0.5 min: `rmqtt.toml default log.dir=/var/log/rmqtt requires root`
- `rmqtt-http-api redb storage path defaults to /var/log/rmqtt/.cache/ which requires root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
