# uteke

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/codecoradev/uteke, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/uteke

## Pinned environment

- Project commit: `7632a852084c536f7910d81dd54d5b8116b19bfe`
- Test commit: `7632a852084c536f7910d81dd54d5b8116b19bfe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.1 to 14.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.9 | 14.1 | 2 | 2 | [run](https://argusic.com/run/5e53cf49-0f84-4a06-b1eb-9f4c2c20c7cb) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `rustc/cargo not installed`
- 0.5 min: `ONNX Runtime library not found at first run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
