# VTCode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vinhnx/VTCode, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/vtcode

## Pinned environment

- Project commit: `01dabf5ac120026f12e5b7568ae7cd65d2f907e3`
- Test commit: `01dabf5ac120026f12e5b7568ae7cd65d2f907e3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 66.5 to 66.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 66.5 | 3 | 3 | [run](https://argusic.com/run/3f516f57-df1c-4080-899e-c8afedfa8e23) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `primary_memory_cache_refreshes_edits_and_missing_files test failed: same-size content not detected as changed (file size too fingerprint was identical)`
- 5 min: `proxy_for_policy unused import warning on Linux (macOS-only symbol)`
- 5 min: `cargo nextest compilation OOM on low-memory system (1GB RAM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
