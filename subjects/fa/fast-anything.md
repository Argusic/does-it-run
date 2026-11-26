# fast-anything

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EL4CTEO/fast-anything, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/fast-anything

## Pinned environment

- Project commit: `ccf46b49daa03799db76bcbb46cacbe873572c1b`
- Test commit: `ccf46b49daa03799db76bcbb46cacbe873572c1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.8 to 19.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 68 | 11.8 | 3 | 3 | [run](https://argusic.com/run/c8d52f0c-b6bb-4208-89be-601d5c6b480e) |
| 2 | pass | 100 | 3 | 19.6 | 1 | 1 | [run](https://argusic.com/run/cfccdbd7-4275-4c21-bcd5-9d8108bde9ea) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Rust toolchain had corrupted/missing components (rustfmt download failed, rustc and cargo binaries missing after initial rustup install)`
- 2 min: `Build failed: can't find crate for 'std' (rust-std component missing)`
- 15 min: `Test failure: python::tests::pool_context_manager_workers_are_profiled_and_recorded - after fork, Pool workers inherit the parent's enabled cProfile.Profile, and sys.setprofile(None) doesn't clear the C-level flag on Python 3.12, causing 'A`

Attempt 2:

- 1.5 min: `test pool_context_manager_workers_are_profiled_and_recorded failed: forked workers inherited parent's active cProfile profiler, causing ValueError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
