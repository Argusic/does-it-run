# lurk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JakWai01/lurk, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/lurk

## Pinned environment

- Project commit: `64a01ebbc71b450ba88f8e41b759aeadd4fcf4fd`
- Test commit: `64a01ebbc71b450ba88f8e41b759aeadd4fcf4fd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 3.1 | 3 | 3 | [run](https://argusic.com/run/f13c1bba-996e-475f-bfcc-a9d51a5af586) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `No Rust toolchain present; installed rustup+stable locally (container lacks system packages via apt).`
- 2 min: `lurk trace failed with 'Unable to set ADDR_NO_RANDOMIZE' because Docker default seccomp denies personality(ADDR_NO_RANDOMIZE) with EPERM (confirmed via C probe and /proc/self/status Seccomp:2).`
- 1 min: `cargo clippy -- -D warnings failed on rustc 1.99 with two 'redundant reference in write!' errors.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
