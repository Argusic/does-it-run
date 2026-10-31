# rustman

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rust-man-org/rustman, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/rustman

## Pinned environment

- Project commit: `5fde2dc34ac055cda13f03d6fa0956d7aecf905b`
- Test commit: `5fde2dc34ac055cda13f03d6fa0956d7aecf905b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 17.7 | 1 | 1 | [run](https://argusic.com/run/bf41d631-8d5f-4a78-92f8-633d6dbc9aef) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain (cargo/rustc) not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
