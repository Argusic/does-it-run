# heh

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ndd7xv/heh, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/heh

## Pinned environment

- Project commit: `89b1e99695069e4caaa3dfb55f90815963a2c3a2`
- Test commit: `89b1e99695069e4caaa3dfb55f90815963a2c3a2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.4 | 1 | 1 | [run](https://argusic.com/run/787ee6d9-1d4d-4fd6-843d-f8d22678650a) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `Terminal narrower than ~10 columns causes arithmetic underflow panic at src/screen.rs:116`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
