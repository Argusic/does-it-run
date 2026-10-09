# intelli-shell

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lasantosr/intelli-shell, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/intelli-shell

## Pinned environment

- Project commit: `fecf5c2ba5ecf648e8e582361f4568f937e014ff`
- Test commit: `fecf5c2ba5ecf648e8e582361f4568f937e014ff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 7 | 3 | 3 | [run](https://argusic.com/run/66605059-fb1a-40b7-885b-f4f695737d4c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed in container`
- 1 min: `cargo clippy - 8 double_must_use errors from async_trait macro`
- 1 min: `cargo +nightly fmt --check failed on 2 files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
