# shodh-memory

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/varun29ankuS/shodh-memory, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/shodh-memory

## Pinned environment

- Project commit: `8ccaf6ab198fa47a9f9d820c640bb72a62273bf3`
- Test commit: `8ccaf6ab198fa47a9f9d820c640bb72a62273bf3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.4 to 21.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 21.4 | 3 | 3 | [run](https://argusic.com/run/4abebab7-aef8-4c41-b2a8-f88e198ee229) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Rust cargo build fails: clang-sys/bindgen/librocksdb-sys needs system libclang development headers (root required)`
- 5 min: `Python native wheel (.abi3.so) segfaults on import via 'cannot allocate memory in static TLS block', and even with LD_PRELOAD workaround, crashes during ONNX model init`
- 1 min: `shodh init downloads a corrupted ONNX Runtime dylib (16KB stub missing OrtGetApiBase)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
