# lla

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chaqchase/lla, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/lla

## Pinned environment

- Project commit: `eb2e7111f7ae69e02d0c475844ef3541bf01339e`
- Test commit: `eb2e7111f7ae69e02d0c475844ef3541bf01339e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.1 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 5.1 | 0 | 0 | [run](https://argusic.com/run/5b24670e-908c-463d-ab1e-9a20df815a8d) |
| 2 | pass | 100 | 8 | 6.5 | 1 | 1 | [run](https://argusic.com/run/db8a286d-2137-4d0f-af08-968ce05ea2f4) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `rust-toolchain.toml listed 9 cross-compilation targets, but rust-std for aarch64-apple-darwin and x86_64-apple-darwin had conflicting rlib files from a previous installation, causing rustup to fail on every build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
