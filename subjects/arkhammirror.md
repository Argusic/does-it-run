# ArkhamMirror

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mantisfury/ArkhamMirror, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/arkhammirror

## Pinned environment

- Project commit: `26e7cd87275c872369c5bfdebbe73d515d459e17`
- Test commit: `26e7cd87275c872369c5bfdebbe73d515d459e17`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 23.2 to 24.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 23.2 | 4 | 4 | [run](https://argusic.com/run/fa730c50-5e7f-41ed-a932-a3bf1e71f091) |
| 2 | pass with mocks | 92 | 24 | 24.9 | 6 | 6 | [run](https://argusic.com/run/5cfef71b-e5e0-4f7f-a539-822907136e75) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pgvector headers missing from extracted pg package`
- 2 min: `Vector dimension mismatch (1024 default vs 384 actual)`
- 1 min: `media-forensics shutdown crashes without callback arg to unsubscribe`
- 1 min: `Pretrained embedding model cannot download (no HF access)`

Attempt 2:

- 4 min: `PostgreSQL not available in container`
- 2 min: `pgvector extension not installed`
- 1 min: `Vector collection dimension mismatch (migration set 1024, default model uses 384)`
- 2 min: `EventBus subscribe/unsubscribe/emit async signature mismatch; tests called methods without await`
- 1 min: `Sequence test assumed increasing order but history stores most-recent-first`
- `8 tests failing due to webhook/scheduler timer-edge-cases and manifest compliance test checking shards not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
