# abtop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/graykode/abtop, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/abtop

## Pinned environment

- Project commit: `4b96568666c1f3b887202d14b0a1c6171315e520`
- Test commit: `4b96568666c1f3b887202d14b0a1c6171315e520`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.8 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 8.8 | 3 | 3 | [run](https://argusic.com/run/741cba9c-2e37-4d91-a3cd-6bdc76d8ae95) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not found`
- `sqlite3 not installed`
- `abtop --help fails with Os error: No such device or address`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
