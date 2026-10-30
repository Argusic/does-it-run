# wingfoil

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wingfoil-io/wingfoil, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/wingfoil

## Pinned environment

- Project commit: `d8204fbad91672ecbd049391d4ad67661af904e3`
- Test commit: `d8204fbad91672ecbd049391d4ad67661af904e3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8 to 8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 2 | 8 | 1 | 0 | [run](https://argusic.com/run/ea65cb9b-cf68-454a-abf6-ea1647138e93) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python crate (wingfoil-python) linking failed: ld cannot find -lpython3.12 (libpython3.12-dev not installed, no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
