# broot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Canop/broot, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/broot

## Pinned environment

- Project commit: `0819142123279d4a03f0c12b689529c4e94fc2bc`
- Test commit: `0819142123279d4a03f0c12b689529c4e94fc2bc`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 3.5 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 24 | 5 | 5 | [run](https://argusic.com/run/97fd6af1-4115-4466-bff7-40873f9eb0d8) |
| 2 | pass | 100 | 3 | 8.2 | 2 | 2 | [run](https://argusic.com/run/8c7ed2d2-4819-4a70-ac11-cd8603148c31) |
| 3 | pass | 100 | 5 | 3.5 | 0 | 0 | [run](https://argusic.com/run/66a53582-2b24-4cbd-84b8-0d295512b75f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain not installed in container`
- 5 min: `No C compiler or build toolchain available (gcc, ld, make, cmake)`
- 2 min: `libc_nonshared.a not found: gcc linker script (libc.so) referenced absolute system path /usr/lib/x86_64-linux-gnu/libc_nonshared.a which didn't exist`
- 2 min: `System headers (stdio.h, limits.h, zlib.h) not found: gcc's #include_next directive searched /usr/include which lacks libc6-dev headers, and libz-sys (test dep via glassbench) failed to compile C source`
- 1 min: `LD_LIBRARY_PATH needed for gcc internal tools (cc1, collect2) to find libisl.so.23`

Attempt 2:

- 0.3 min: `No Rust toolchain found in environment`
- 1 min: `Termimad IO error (os error 6) and keyboard enhancement timeout when running TUI mode without a real PTY`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
