# lowfat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zdk/lowfat, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/lowfat

## Pinned environment

- Project commit: `a17b3e0602c954a8160abc9086085083ad2405d5`
- Test commit: `a17b3e0602c954a8160abc9086085083ad2405d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.3 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 5.4 | 0 | 0 | [run](https://argusic.com/run/a4ff7d71-aeeb-4216-b54e-9496f5263552) |
| 2 | pass | 100 | 3 | 4.3 | 1 | 1 | [run](https://argusic.com/run/72d92a14-19e8-4adf-ae7a-41c6fd286294) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not installed (rustc, cargo not found in PATH)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
