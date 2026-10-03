# bili-sync

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amtoaer/bili-sync, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/bili-sync

## Pinned environment

- Project commit: `cc9a77aa493471474ff2b29c88b8646cd57bf276`
- Test commit: `cc9a77aa493471474ff2b29c88b8646cd57bf276`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.4 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.5 | 0 | 0 | [run](https://argusic.com/run/dbb8619c-12b4-4241-a18d-cc352b67054b) |
| 2 | pass | 100 | 6 | 7.4 | 3 | 3 | [run](https://argusic.com/run/e47ea265-cb42-4328-9a23-ca3ebf0d3461) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not installed`
- 1 min: `Node.js v18 was too old for frontend build dependencies (required ^20.19.0)`
- `npm install failed due to engine conflict with @eslint/compat`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
