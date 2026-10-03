# veloren

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/veloren/veloren, licensed GPL-3.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/veloren

## Pinned environment

- Project commit: `3ca2c1920f72793197c61efae74561ee317e4027`
- Test commit: `3ca2c1920f72793197c61efae74561ee317e4027`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 42 to 90.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 28 | 48.6 | 2 | 1 | [run](https://argusic.com/run/0954bab0-70bb-4e42-858e-f895b207c302) |
| 1 | pass | 100 | 31 | 90.8 | 2 | 2 | [run](https://argusic.com/run/44c84dfa-5012-4607-ba1a-6ea56427ef9c) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/6cc2b50f-05fb-447e-bf49-8ee803a295f5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `cargo config specified mold linker not available in container`
- 1 min: `voxygen client requires alsa-sys/libasound2-dev which needs root to install`

Attempt 1:

- 1 min: `.cargo/config.toml specifies mold linker which is not installed`
- 2 min: `libasound2-dev and libudev-dev packages not installed (no root access), missing .pc files and .so symlinks for link-time`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
