# selfgraph

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hydra-db/selfgraph, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/selfgraph

## Pinned environment

- Project commit: `97fb52be8e8ef69b7c43bf47f7ca07f44b500d6d`
- Test commit: `97fb52be8e8ef69b7c43bf47f7ca07f44b500d6d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 48.3 to 48.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 0.4 | 48.3 | 2 | 1 | [run](https://argusic.com/run/cf90348e-3cc7-4b29-b0dc-f7fdd81f2c4e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `kuzu 0.11.3 needs a larger buffer pool than 64MB for 513 relation versions`
- 2 min: `test_kuzu_cancel_then_close subprocess OOM-killed (SIGKILL -9) on container with ~1GB RAM: spawns 50 Kuzu databases at 128MB each`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
