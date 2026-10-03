# quickwit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/quickwit-oss/quickwit, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/quickwit

## Pinned environment

- Project commit: `af0591a36e16831af9a2ad9484e12465f511ef84`
- Test commit: `af0591a36e16831af9a2ad9484e12465f511ef84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.9 to 35.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 35.9 | 6 | 6 | [run](https://argusic.com/run/e221a32c-34d0-4ff8-bd2d-e4396d0402a6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 1 min: `protoc not installed`
- 4 min: `cargo-nextest not installed`
- `pre-existing test failure: test_concatenate_multiple_field returns values in wrong order`
- `Docker not available; integration tests requiring Docker services (S3, Kafka, Postgres) skipped`
- `make fmt requires nightly toolchain`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
