# Douyin_TikTok_Download_API

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Evil0ctal/Douyin_TikTok_Download_API, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/douyin-tiktok-download-api

## Pinned environment

- Project commit: `bcbbfa17dcea6dcbe93a5a985155a61ad1227cf2`
- Test commit: `bcbbfa17dcea6dcbe93a5a985155a61ad1227cf2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 34.2 to 48 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 37 | 38.1 | 7 | 7 | [run](https://argusic.com/run/7c93cfaf-cd43-4a08-adae-6f3f1ff5b000) |
| 2 | pass with mocks | 92 | 52 | 34.2 | 5 | 5 | [run](https://argusic.com/run/51af5bdf-6a88-44b0-a0e7-cfc1f1911d92) |
| 3 | pass | 100 | 2 | 48 | 6 | 6 | [run](https://argusic.com/run/198bbf94-f7ae-410d-a851-425647f0646c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not found (missing from PATH)`
- 0.5 min: `DTK_SECRET_KEY not set causing unit test failures`
- 10 min: `Docker not available; cannot use docker compose for Postgres/Redis`
- 8 min: `TimescaleDB from apt has Apache-only license restricting add_retention_policy etc.`
- 5 min: `TimescaleDB loader .so vs extension .so confusion (wrong binary used for shared_preload_libraries)`
- 2 min: `Node 18 too old for web console build (rolldown requires Node 20+/22+)`
- 3 min: `Downloader Go binary not built (needed by integration tests)`

Attempt 2:

- 1 min: `Missing .env with DTK_SECRET_KEY caused 7 test failures`
- 25 min: `No Docker - cannot use compose.yml for PostgreSQL/Redis`
- `Integration test test_docs_belongs_to_the_console_not_to_swagger fails (404 vs 200)`
- `24 downloader integration tests fail`
- `4 console integration tests fail`

Attempt 3:

- 1 min: `uv not installed`
- 1 min: `DTK_SECRET_KEY not set, 7 unit tests failed`
- 5 min: `TimescaleDB extension not available for PostgreSQL, migration and 7 integration tests failed`
- 1 min: `Redis auth required by tests, 17 e2e tests errored`
- 3 min: `Console SPA web/dist not built, 4 integration tests failed`
- 3 min: `Go downloader sidecar not built, 24 download integration tests failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
