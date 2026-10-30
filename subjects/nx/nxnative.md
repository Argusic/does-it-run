# nxnative

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/seedds/nxnative, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nxnative

## Pinned environment

- Project commit: `ac9598ad83e2706881568cafe345d262459ccd05`
- Test commit: `ac9598ad83e2706881568cafe345d262459ccd05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.5 to 14.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 19 | 14.5 | 1 | 1 | [run](https://argusic.com/run/e8b47cc5-b447-4609-a11d-f5a42df1d684) |
| 2 | pass | 100 | 12 | 6.5 | 5 | 5 | [run](https://argusic.com/run/cf4ee83a-3a33-402c-b389-b1dfcc68450b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_romfs_image.py C compilation failed on Linux GCC 13 -Wmisleading-indentation (bare if bodies without braces)`

Attempt 2:

- 1 min: `Pip could not install into system Python (externally-managed-environment)`
- 3 min: `Missing Python deps: lz4, capstone, fonttools, zstd, backports.zstd`
- 1 min: `gcc-13 -Wmisleading-indentation error on one-liner C in test_romfs_image.py`
- `Pre-existing flaky test test_romfs_image.py::test_reuse_rebuilds_changed_added_removed_and_renamed_files (ext4 ctime resolution)`
- `test_spirv_cross_pin, test_nsp_mac_app, test_own_compilers, test_regress need macOS/Xcode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
