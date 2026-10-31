# RelaMind

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/El-12stu/RelaMind, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/relamind

## Pinned environment

- Project commit: `40ef0f3c027dacc3160386a5fbdfc563d28bb2b3`
- Test commit: `40ef0f3c027dacc3160386a5fbdfc563d28bb2b3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.9 to 34.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 34 | 34.9 | 5 | 5 | [run](https://argusic.com/run/a8288c7b-3278-4094-ba1a-5d4076c5820f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java 21 not available in environment`
- 2 min: `DashScope API key missing for Spring context tests`
- 8 min: `Cassandra repositories missing - Spring context failed to load`
- 10 min: `VectorStore and RAG cloud advisor configs triggered real API calls`
- 3 min: `PgVector VectorStore not available (no PostgreSQL)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
