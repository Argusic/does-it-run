# Albatross

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/morganlinton/Albatross, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/albatross

## Pinned environment

- Project commit: `e458e4277f463a4688f127ea6ea61f5a344b64b8`
- Test commit: `e458e4277f463a4688f127ea6ea61f5a344b64b8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.6 to 17.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 17.6 | 3 | 3 | [run](https://argusic.com/run/46cb0e07-61c9-4661-a596-6a0a86df27e7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 2 min: `cargo clippy failed with clippy::double_must_use on Rust 1.99 (new lint on async_trait)`
- 1 min: `cargo fmt caught extra blank line after the allow annotation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
