# ibis

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ibis-project/ibis, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ibis

## Pinned environment

- Project commit: `05d2b293344e86cb41c1a426071734f7e270335a`
- Test commit: `05d2b293344e86cb41c1a426071734f7e270335a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.3 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.3 | 0 | 0 | [run](https://argusic.com/run/038bffc4-cfc7-4262-83ed-1f17ad36a90c) |
| 2 | pass | 100 | 45 | 8.5 | 3 | 3 | [run](https://argusic.com/run/d5c7fced-2270-4f1e-a16c-cd3a4518e441) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `mysqlclient build failure when using --all-extras: missing libmysqlclient system headers`
- 1 min: `Missing test data directory ci/ibis-testing-data (gitignored, not in repo)`
- 1 min: `Missing black for decompile_tpch tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
