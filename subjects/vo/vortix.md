# vortix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Harry-kp/vortix, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/vortix

## Pinned environment

- Project commit: `a1071eef57231f37b3c2290a8aefa599a0df7105`
- Test commit: `a1071eef57231f37b3c2290a8aefa599a0df7105`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28 to 28 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 28 | 2 | 2 | [run](https://argusic.com/run/677e089e-af2b-473e-b078-e2cd008a4d95) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 8 min: `18 test failures due to process umask 0002 causing group-writable tempdirs rejected by security checks`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
