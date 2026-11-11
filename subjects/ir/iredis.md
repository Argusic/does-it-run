# iredis

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/laixintao/iredis, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/iredis

## Pinned environment

- Project commit: `554bff6bfaa499e8fce488fb9dbd21900cd3d0ba`
- Test commit: `554bff6bfaa499e8fce488fb9dbd21900cd3d0ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.6 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.6 | 3 | 3 | [run](https://argusic.com/run/be8bb8c2-f1fe-4ad9-88e8-62e647bb4d7a) |
| 2 | pass | 100 | 5 | 8.7 | 3 | 3 | [run](https://argusic.com/run/7bfdc73d-3abf-495e-b670-0ed00eb8bdcf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 blocks system pip install`
- 2 min: `no redis-server binary in container`
- 0.5 min: `REDIS_VERSION env var not set`

Attempt 2:

- 1 min: `PEP 668 prevents pip from installing poetry system-wide`
- 2 min: `No redis-server binary in container`
- 1 min: `Fakeredis zombie process bound to port 6379 blocked real redis-server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
