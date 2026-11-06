# sd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chmln/sd, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/sd

## Pinned environment

- Project commit: `44febdf86343c653255ae4f20f5e1882dad6be17`
- Test commit: `44febdf86343c653255ae4f20f5e1882dad6be17`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 2.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 2 | 0 | 0 | [run](https://argusic.com/run/65fbe864-e2e4-4e38-80d4-c773588f0b92) |
| 2 | pass | 100 | 2 | 2.5 | 2 | 2 | [run](https://argusic.com/run/7997c76d-2203-4a36-8951-1f3c24cbbe13) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `No Rust toolchain (rustc/cargo) present in container`
- 0.5 min: `cargo install sd --path sd-cli failed: could not find 'sd' in /work/repo/sd-cli (package name mismatch)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
