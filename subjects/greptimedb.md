# greptimedb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GreptimeTeam/greptimedb, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/greptimedb

## Pinned environment

- Project commit: `194bc2fb3c48ea1c55cff8fdd5886daa8b60d8ad`
- Test commit: `194bc2fb3c48ea1c55cff8fdd5886daa8b60d8ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 82.3 to 82.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 80 | 82.3 | 6 | 6 | [run](https://argusic.com/run/8a97e404-4b26-48c5-b3d3-3dd1600bd6f8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed`
- 1 min: `protoc not installed`
- 1 min: `protoc missing google include files`
- 3 min: `substrait build script failed (google/protobuf/any.proto not found)`
- 30 min: `rustc SIGSEGV in LLVM AsmPrinter::emitFunctionBody during parallel compilation`
- 5 min: `Disk space exhausted (40GB overlay, 99% full) from repeated build artifacts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
