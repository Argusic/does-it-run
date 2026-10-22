# sdk-rust

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/temporalio/sdk-rust, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/sdk-rust

## Pinned environment

- Project commit: `0eb03f213079e539c18fb738c32a70bc191aadf4`
- Test commit: `0eb03f213079e539c18fb738c32a70bc191aadf4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 76 to 76 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 76 | 6 | 6 | [run](https://argusic.com/run/0493662d-602b-4273-831a-73695ddb9dc7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain installed`
- 1 min: `Missing protoc protobuf compiler`
- `protoc could not find google/protobuf/field_mask.proto`
- 1 min: `IPv6 disabled in container causing connection_uses_http_connect_proxy test failure`
- `trybuild stderr file mismatch due to Rust 1.94 shorter note paths (no crate prefix)`
- 1 min: `Disk ran out of space (40G) during integration test compilation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
