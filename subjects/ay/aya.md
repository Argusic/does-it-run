# aya

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aya-rs/aya, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/aya

## Pinned environment

- Project commit: `df926b48e958e96ca7474f09c6db9ec1ed16eb7a`
- Test commit: `df926b48e958e96ca7474f09c6db9ec1ed16eb7a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 6.1 | 1 | 1 | [run](https://argusic.com/run/5e15fb57-fdc2-443a-8ed6-812745fd53dd) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Tests failed: ProcMapEntry inode field overflowed on overlayfs (inode 16648323018 > u32::MAX)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
