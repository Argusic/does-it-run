# logfire

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pydantic/logfire, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/logfire

## Pinned environment

- Project commit: `84ff5dfba6dbc5ab46e14ee4a11acb2229812b44`
- Test commit: `84ff5dfba6dbc5ab46e14ee4a11acb2229812b44`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 44.7 to 71.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 71.1 | 4 | 4 | [run](https://argusic.com/run/2ef44daf-5865-4139-b588-4899b877fab5) |
| 2 | pass | 100 | 0.5 | 44.7 | 0 | 0 | [run](https://argusic.com/run/1db82a09-d77a-4d09-b160-d1bc7cef1f07) |
| 3 | pass with mocks | 92 | 1 | 51.3 | 2 | 2 | [run](https://argusic.com/run/62a0709d-986f-49ef-b70c-077be7e2daa7) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not pre-installed`
- `Snapshot test failures in VCR-based LLM integration tests (pre-existing, caused by dependency version drift between recorded cassettes and current library versions)`
- `Docker-based tests (pymongo, redis, celery, mysql, asyncpg, psycopg, surrealdb, sqlalchemy) cannot run without Docker`
- `Test suite hanging when run with xdist (-n logical) - pre-existing issue with process-level isolation`

Attempt 3:

- 1 min: `pytest-anyio not installed (missing dependency in uv.lock)`
- 1 min: `Inline snapshot failures in test_otel_logs.py (2 tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
