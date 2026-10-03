# sem

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ataraxy-Labs/sem, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/sem

## Pinned environment

- Project commit: `55ba2f1d8fc6ce657711b0deb10d21eb5c0ddb49`
- Test commit: `55ba2f1d8fc6ce657711b0deb10d21eb5c0ddb49`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14.7 | 24 | 1 | 1 | [run](https://argusic.com/run/c09b3c77-505b-4b65-a94a-c3f78337dc73) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Flaky test persist::disk_cache::tests::precomputed_columns_match_internal_fusion intermittently fails with SqliteFailure(SystemIoFailure) when running in parallel , tempfs contention in the test harness's temp_repo_root function`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
