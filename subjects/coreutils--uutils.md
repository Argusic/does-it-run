# coreutils

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/uutils/coreutils, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/66c58645-5c16-47e4-957c-ac3de60d9773

## Pinned environment

- Project commit: `ddc98c2547448e43cb58736048103f4ab6a07f82`
- Test commit: `ddc98c2547448e43cb58736048103f4ab6a07f82`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 10.5 to 26.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25.6 | 26.7 | 6 | 6 | [run](https://argusic.com/run/66c58645-5c16-47e4-957c-ac3de60d9773) |
| 2 | pass | 100 | 12 | 10.5 | 6 | 6 | [run](https://argusic.com/run/af9b732a-ba13-4353-88d6-3b698907de59) |
| 3 | pass | 100 | 6.17 | 24.3 | 5 | 5 | [run](https://argusic.com/run/4f677db3-971d-4aaf-b1bd-1b1ece6c1b5f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain (rustc, cargo) not installed in container`
- 8 min: `No C compiler/linker (cc) found for Rust build scripts and linking`
- 5 min: `No ar (archiver) found for build scripts`
- 0.5 min: `3 cp sparse tests fail on overlay filesystem (blocks count mismatch)`
- `1 touch 2-digit-year test fails (year 68 parsed as 2038 instead of 2068)`
- `1 touch stdin-test fails (race condition on mtime update)`

Attempt 2:

- 0.3 min: `Rust toolchain not pre-installed`
- `test_localization_and_colors: 3 ANSI color tests fail in headless environment (b2sum help/error colors)`
- `test_cp::test_cp_sparse_always_empty: assertion failed (left: 32, right: 0)`
- `test_cp::test_cp_sparse_always_non_empty: assertion failed (left: 136, right: 16)`
- `test_cp::test_cp_debug_reflink_auto_sparse_always_non_sparse_file_with_long_zero_sequence: assertion failed (left: 40, right: 8)`
- `test_ls::test_device_number: panicked expecting block/char device`

Attempt 3:

- 2.5 min: `rustc not found in container`
- `test_localization_and_colors: 3 tests fail because no TTY attached so ANSI color codes are not emitted`
- `test_ls::test_device_number: no block/char devices in /dev in container`
- `test_cp sparse tests: overlay FS doesn't support block reporting`
- `47 tail follow tests fail: inotify "Too many open files" / cannot be used in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
