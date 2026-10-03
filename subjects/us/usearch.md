# USearch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unum-cloud/USearch, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/usearch

## Pinned environment

- Project commit: `f91fe5bc000222aa1af6e91daf78c2bb20b0c90e`
- Test commit: `f91fe5bc000222aa1af6e91daf78c2bb20b0c90e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.1 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 18.1 | 2 | 2 | [run](https://argusic.com/run/0fd3d717-8a1c-4f00-aba3-cddfd782f93f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Python.h not found (python3-dev not installed) preventing C++ extension build from source`
- 4 min: `usearch.sqlite_path() referenced non-existent binary for SQLite extension`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
