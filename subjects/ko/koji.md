# koji

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cococonscious/koji, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/koji

## Pinned environment

- Project commit: `9a0b96e18f71510a87acc8376ce254ca7a31b62b`
- Test commit: `9a0b96e18f71510a87acc8376ce254ca7a31b62b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8 | 1 | 1 | [run](https://argusic.com/run/23333ac3-2947-4e2e-8a54-90da0c40be80) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain (cargo/rustc) not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
