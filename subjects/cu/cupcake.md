# cupcake

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eqtylab/cupcake, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/cupcake

## Pinned environment

- Project commit: `27b94b84f6cf555bfde5817deae323ee8cb00cea`
- Test commit: `27b94b84f6cf555bfde5817deae323ee8cb00cea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 18.7 | 2 | 2 | [run](https://argusic.com/run/aa7fea25-a85c-48b4-aad9-b37d2945647c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
