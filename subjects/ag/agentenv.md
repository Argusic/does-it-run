# AgentENV

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kvcache-ai/AgentENV, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/agentenv

## Pinned environment

- Project commit: `5843159b1eaf235a45a08a5329fc6647c6e5bc31`
- Test commit: `5843159b1eaf235a45a08a5329fc6647c6e5bc31`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.9 to 41.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 36 | 41.9 | 5 | 4 | [run](https://argusic.com/run/b4cd6ee8-b90f-4a40-b06b-f50e7a06e8d3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed`
- 3 min: `libclang not found (bindgen dependency)`
- 2 min: `stdbool.h not found (rocksdb-sys dependency)`
- 1 min: `protoc not found (prost-build dependency)`
- `6 overlaybd direct-I/O tests fail in container (O_DIRECT unsupported on tmpfs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
