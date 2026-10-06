# tuxedo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/webstonehq/tuxedo, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tuxedo

## Pinned environment

- Project commit: `de7c0dbbc78601ad5e742b7907ce24b809d65be3`
- Test commit: `de7c0dbbc78601ad5e742b7907ce24b809d65be3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.5 to 3.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 3.5 | 1 | 1 | [run](https://argusic.com/run/e88eca38-f773-4cc5-9802-3dac27bb2e86) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Rust toolchain not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
