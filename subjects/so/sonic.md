# sonic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/valeriansaliou/sonic, licensed MPL-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/sonic

## Pinned environment

- Project commit: `c0f3ff9dbcbd0fc6a6daf0a9d2f311f7d68f0b1a`
- Test commit: `c0f3ff9dbcbd0fc6a6daf0a9d2f311f7d68f0b1a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.9 to 35.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 35.7 | 5 | 5 | [run](https://argusic.com/run/591e0651-5d8c-4170-a0ca-307f6a3b1ac5) |
| 2 | pass | 100 | 18 | 17.9 | 3 | 3 | [run](https://argusic.com/run/052b3081-f99a-4538-9e76-586ccc75ed8c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `rustc/cargo not found in container`
- 8 min: `librocksdb-sys build fails: libclang not found`
- 2 min: `librocksdb-sys build fails: stdbool.h not found by clang`
- 1 min: `Server cannot bind to IPv6 [::1]:1491 (container has IPv6 disabled)`
- 1 min: `Client tests fail because they hardcode Ipv6Addr::LOCALHOST`

Attempt 2:

- 2 min: `libclang shared library not found`
- 1 min: `stdbool.h not found in libclang include path`
- 3 min: `IPv6 loopback unavailable in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
