# rushdb

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rush-db/rushdb, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/rushdb

## Pinned environment

- Project commit: `0986694ab96539d8097ca8975c8bc955030e1ab5`
- Test commit: `0986694ab96539d8097ca8975c8bc955030e1ab5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 43 to 80.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 80.1 | 0 | 0 | [run](https://argusic.com/run/2b993fcd-8eca-4776-8913-0289e404414b) |
| 2 | pass | 100 | 43 | 43 | 1 | 1 | [run](https://argusic.com/run/b161ec87-e730-4677-83ba-f3d1fcef8b25) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `No Rust toolchain (rustup, cargo, rustc) was installed in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
