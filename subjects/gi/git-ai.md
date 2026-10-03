# git-ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/git-ai-project/git-ai, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/git-ai

## Pinned environment

- Project commit: `1f16720db8553f19622fa83e728a8247ff825727`
- Test commit: `1f16720db8553f19622fa83e728a8247ff825727`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 29.3 to 45.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 29.3 | 2 | 2 | [run](https://argusic.com/run/7cdb26d2-45bb-49a5-96a5-91e56568fb96) |
| 2 | pass | 100 | 38 | 45.3 | 3 | 3 | [run](https://argusic.com/run/9bc7a7e5-285f-4a90-8e70-8463cd567a49) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Rust 1.98.1 clippy rules treated 12 warnings as errors that were not issues with the target Rust 1.93.0`
- 2 min: `array_chunks() and as_chunks() are stable-only in Rust 1.80+/1.97+`

Attempt 2:

- 17 min: `No Rust toolchain installed`
- 1 min: `Integration tests fail: rustup cargo proxy not found in subprocess`
- 5 min: `Cargo file lock contention from overlapping builds`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
