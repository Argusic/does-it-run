# ai-memory

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/akitaonrails/ai-memory, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ai-memory

## Pinned environment

- Project commit: `49147a5d173657031b6b846e5beb8a839219c050`
- Test commit: `49147a5d173657031b6b846e5beb8a839219c050`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 85.3 to 85.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 60 | 85.3 | 4 | 4 | [run](https://argusic.com/run/66b4137f-49a9-4d1f-86f3-fffcbc55cd72) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust 1.95 toolchain not pre-installed in container`
- 5 min: `Lock contention from concurrent cargo build processes (LTO/test builds)`
- 2 min: `MCP test binary (101 MB LTO build) required >120s, got killed by timeout`
- 1 min: `cargo t alias requires cargo-nextest but cargo-nextest was not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
