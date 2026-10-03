# tonbo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tonbo-io/tonbo, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/tonbo

## Pinned environment

- Project commit: `f95b9e0d6f3d317e8a44f683881c2a19e02e2a4d`
- Test commit: `f95b9e0d6f3d317e8a44f683881c2a19e02e2a4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.6 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6.6 | 1 | 1 | [run](https://argusic.com/run/a41f7964-afe4-49d9-8e5a-7a9854499e17) |
| 2 | pass | 100 | 9 | 8.8 | 0 | 0 | [run](https://argusic.com/run/a63a6602-4612-4aa4-8843-659e999f5d3d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Rust toolchain installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
