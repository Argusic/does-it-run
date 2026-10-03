# zoxide

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ajeetdsouza/zoxide, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/zoxide

## Pinned environment

- Project commit: `416584909585a00d0c2204f83d11c42e4497bb93`
- Test commit: `416584909585a00d0c2204f83d11c42e4497bb93`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 3.2 to 28.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 31 | 28.8 | 3 | 3 | [run](https://argusic.com/run/8d4482da-bd66-4242-a13d-b6e548509d73) |
| 2 | pass | 100 | 2 | 5.1 | 0 | 0 | [run](https://argusic.com/run/71a65a40-30c5-400e-b3df-dd410b926bd4) |
| 3 | pass | 100 | 0.3 | 3.2 | 0 | 0 | [run](https://argusic.com/run/b88df33f-bf26-464e-8624-8eb5e9d186a7) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `No C compiler (cc) or Rust toolchain installed in container`
- 10 min: `Rust build scripts failed linking with 'cc not found'`
- 5 min: `ld.lld/rust-lld failed linking due to missing libc_nonshared.a, libm-2.39.a, and libmvec.a with hardcoded paths in linker scripts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
