# agno

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agno-agi/agno, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agno

## Pinned environment

- Project commit: `660c0ee8c5cc0cbc1bc93d66dac110f90740fd96`
- Test commit: `660c0ee8c5cc0cbc1bc93d66dac110f90740fd96`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 42.6 to 62.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 42.6 | 6 | 6 | [run](https://argusic.com/run/5854a61f-16c7-4915-93f4-9251f3755223) |
| 2 | pass with mocks | 78.67 | 12 | 62.2 | 6 | 2 | [run](https://argusic.com/run/0e9092b4-0e8f-42a2-9d6c-9d14123e5c1d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Disk space insufficient to install 'agno[tests]' extra (torch/triton ~5GB)`
- 1 min: `Missing google-api-python-client for gdrive mime types test (collection error)`
- 1 min: `Missing pymongo for async mongo DB test (collection error)`
- 1 min: `22 tool test files failed collection (cassio, oxylabs, crawl4ai, chonkie, cartesia, etc. not installed)`
- `12 workflow test_run_logging tests fail (assert 0 == 1 - pre-existing, not caused by install)`
- `109 total collection errors across vectordb, models, reader, knowledge, db, os, fs, context test dirs`

Attempt 2:

- 8 min: `Missing dependencies (39 total package install rounds needed)`
- `60 pre-existing mypy type errors in agno library`
- `test_async_mongo.py hangs (needs real MongoDB)`
- `3 pre-existing vectordb test failures`
- `10 pre-existing learn/ test failures`
- `PDF reader tests fail (pypdf API change)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
