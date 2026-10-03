# lancedb

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lancedb/lancedb, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/lancedb

## Pinned environment

- Project commit: `22165860231231d738c246ccd4d0ef46f5baedd8`
- Test commit: `22165860231231d738c246ccd4d0ef46f5baedd8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 84.4 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/c4adeed5-dc29-4108-a0f6-2edc5f4c94e1) |
| 2 | pass | 96 | 22 | 84.4 | 5 | 4 | [run](https://argusic.com/run/1320747e-791f-4546-b6a3-8b887832656c) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not installed`
- 1 min: `protoc not found`
- 1 min: `No space left on device (disk full)`
- 1 min: `uv not found on PATH`
- `TypeScript build requires Node.js >=22 but container has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
