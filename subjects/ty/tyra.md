# tyra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/h4570/tyra, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/tyra

## Pinned environment

- Project commit: `c59f406af134713b62656114846ac8d588c6247c`
- Test commit: `c59f406af134713b62656114846ac8d588c6247c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.8 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 24.8 | 5 | 5 | [run](https://argusic.com/run/53092b47-a0be-4f81-bbad-22f12f211485) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing PS2DEV cross-compiler toolchain - Docker-based install requires Docker which is unavailable`
- 8 min: `VCL (32-bit ELF binary) cannot run - no 32-bit glibc or QEMU installed`
- 2 min: `VCLPP not available - needs to be built from source`
- 2 min: `bin2s tool missing in pre-built PS2SDK`
- 1 min: `std::function used with missing #include <functional> in renderer_3d_pipeline.hpp`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
