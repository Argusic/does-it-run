# reqwest

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/seanmonstar/reqwest, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/reqwest

## Pinned environment

- Project commit: `aff2ddb677e20517baec5254b8800c6d371aa010`
- Test commit: `aff2ddb677e20517baec5254b8800c6d371aa010`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 37.1 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/4cb17980-d026-4944-8bb4-ede3e1c54806) |
| 2 | pass | 100 | 0.7 | 37.1 | 1 | 1 | [run](https://argusic.com/run/35539d6c-13ac-46b9-9c97-a8789a774dc8) |

## What was observed on a clean machine

Attempt 2:

- `Disk full (7.8 GB root) when compiling with optional features (blocking, cookies, gzip, brotli, deflate, zstd, multipart). Linker failed with 'No space left on device' during cargo test on extended feature set.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
