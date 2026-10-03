# libsql

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tursodatabase/libsql, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/libsql

## Pinned environment

- Project commit: `d6c75af6353bb1c34985399608e37cd272a35aa1`
- Test commit: `d6c75af6353bb1c34985399608e37cd272a35aa1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 18.4 to 31.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29 | 31.9 | 3 | 3 | [run](https://argusic.com/run/c9d20ef7-de09-4588-80f7-dbe56a04bf66) |
| 2 | pass | 100 | 3 | 18.4 | 1 | 1 | [run](https://argusic.com/run/465d1be1-5b2d-4b50-8d71-001d2a5dcddf) |
| 3 | pass | 100 | 21 | 29.4 | 3 | 3 | [run](https://argusic.com/run/d6874834-b7d3-4ae1-9470-b0425bdefe8c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `rustc: not found , Rust toolchain not installed`
- 1 min: `cargo xtask build: configure requires tclConfig.sh for TCL (C library build path only)`
- 1 min: `libsql_replication bootstrap test needs protoc (protobuf compiler)`

Attempt 2:

- 1 min: `Missing protoc compiler for libsql_replication bootstrap integration test`

Attempt 3:

- 1 min: `Rust toolchain not installed (no rustc, cargo, rustup)`
- 1 min: `protoc not installed, needed by libsql_replication test build.rs`
- `3 libsql-server tests failed (attach_auth, attach_auth_with_uuids, basic_metrics)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
