# OpenAgentd

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lthoangg/OpenAgentd, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openagentd

## Pinned environment

- Project commit: `d44ddffc5b21a278f5e3fd70183426bad49eb19f`
- Test commit: `d44ddffc5b21a278f5e3fd70183426bad49eb19f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.9 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 19.9 | 4 | 4 | [run](https://argusic.com/run/d7d963de-e5a5-4c94-8048-d0481c3f67c8) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `uv, bun, and unzip/npm-global were missing; system Node 18 too old for the web build (rolldown imports node:util styleText); desktop install.sh requires apt+sudo which are unavailable in the container`
- 4 min: `Fresh first-run server start (make run / uvicorn, APP_ENV=development) crashed: no such table: scheduled_task because auto-migration only runs in production`
- 8 min: `tests/services/test_observability_service.py::test_summary_cache_invalidates_when_span_files_change failed: observability _run_queries call_count was 4 instead of 5; root cause: cache signature (path,size,mtime_ns,inode) did not detect appe`
- 1 min: `First end-to-end chat attempt hit ConnectError 5x because the backgrounded mock LLM process was reaped when its exec session ended`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
