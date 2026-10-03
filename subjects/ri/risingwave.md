# risingwave

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/risingwavelabs/risingwave, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/risingwave

## Pinned environment

- Project commit: `d0fcaa90a5e12c88041731c1ced535b53be26299`
- Test commit: `d0fcaa90a5e12c88041731c1ced535b53be26299`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 57.2 to 57.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 47 | 57.2 | 4 | 4 | [run](https://argusic.com/run/3406f1fc-3a16-479e-9afb-7a8c8b9f7c19) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed`
- 1 min: `protoc not found`
- 16 min: `faiss-sys cmake build fails , no Fortran compiler / BLAS not found`
- 3 min: `OOM killed during parallel compilation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
