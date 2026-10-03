# gitlogue

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unhappychoice/gitlogue, licensed ISC, written in Rust.

Evidence and recordings: https://argusic.com/subject/gitlogue

## Pinned environment

- Project commit: `73750f745249e72874ee7118469ce847aab24955`
- Test commit: `73750f745249e72874ee7118469ce847aab24955`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 4.3 to 30.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29.5 | 30.5 | 9 | 9 | [run](https://argusic.com/run/8691da58-6fe2-47c9-a196-84590a0390c5) |
| 2 | pass | 100 | 8 | 5 | 0 | 0 | [run](https://argusic.com/run/bdcde4da-beff-4a41-82bc-2a32fdb387bd) |
| 3 | pass | 100 | 3.3 | 4.3 | 0 | 0 | [run](https://argusic.com/run/3020d709-1a10-490b-b046-dfa3f0e295b3) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Rust toolchain not installed`
- 5 min: `No C compiler (gcc/cc) found on system`
- 1 min: `libbfd-2.42-system.so not found by linker`
- 2 min: `Missing crtbeginS.o and libgcc_s.so.1`
- 1 min: `libc.so linker script has absolute paths (/usr/lib/x86_64-linux-gnu/libc_nonshared.a)`
- 0.5 min: `libm.so linker script has absolute paths`
- 0.5 min: `OpenSSL build failed: 'make' not found`
- 1 min: `OpenSSL build failed: missing system headers (stdlib.h, limits.h)`
- 1 min: `libisl.so.23, libmpc.so.3, libmpfr.so.6 not found by cc1/cc1plus`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
