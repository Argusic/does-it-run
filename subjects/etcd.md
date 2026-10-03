# etcd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/etcd-io/etcd, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/etcd

## Pinned environment

- Project commit: `e9e56564d6f13af87747cdb785bc1832791090b4`
- Test commit: `e9e56564d6f13af87747cdb785bc1832791090b4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 8.9 to 23.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 17.3 | 1 | 1 | [run](https://argusic.com/run/2e5da4b8-39b7-41a2-be8a-84b333efe51d) |
| 2 | pass | 100 | 23 | 23.2 | 2 | 2 | [run](https://argusic.com/run/3a20515a-dea8-4d12-bf94-505b222aede2) |
| 3 | pass | 100 | 10 | 8.9 | 2 | 2 | [run](https://argusic.com/run/f450a2b6-e967-4ff4-acce-0f8f8f942469) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.26.7 required but not preinstalled in container`

Attempt 2:

- 3 min: `Go 1.26.7 not installed in container`
- 2 min: `Background etcd process exited when parent shell ended`

Attempt 3:

- 1 min: `Test TestReadWriteTimeoutDialer failed: 5MB write buffer fit in Linux socket buffer without blocking, so no write timeout occurred`
- 1 min: `Test TestWriteReadTimeoutListener failed: same root cause as above`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
