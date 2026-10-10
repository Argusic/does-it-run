# workflow

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/durable-workflow/workflow, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/workflow

## Pinned environment

- Project commit: `210682a4c40558273b483e037b17a8ca62e9d463`
- Test commit: `210682a4c40558273b483e037b17a8ca62e9d463`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42.8 to 42.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 45 | 42.8 | 4 | 3 | [run](https://argusic.com/run/12857787-a69f-4f64-bf29-6df488a586e7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP and Composer not pre-installed in container`
- 5 min: `PostgreSQL and Redis not available as services`
- 2 min: `Unit tests failed (531 errors) before infrastructure was available due to missing DB/Redis`
- `3 ProjectionPrefetchTest failures due to PostgreSQL 16 trailing-zero timestamp format difference (.450480 vs .45048)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
