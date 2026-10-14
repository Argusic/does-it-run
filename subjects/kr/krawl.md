# Krawl

**Verdict: not yet verified.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BlessedRebuS/Krawl, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/krawl

## Pinned environment

- Project commit: `5b37247c4950d183f71338ecd07dd6a28d6f4955`
- Test commit: `5b37247c4950d183f71338ecd07dd6a28d6f4955`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.6 to 35.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 40 | 35.6 | 5 | 5 | [run](https://argusic.com/run/c7dbdcd7-f777-470c-adaa-af6454afe976) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `py-tlsh wheel build failed: missing Python.h (python3-dev not installed, no root); no prebuilt cp312 wheel on PyPI`
- 3 min: `tests/test_map_tiles.py expected old ?key= param, code now emits ?api_key=`
- 2 min: `tests/test_startup_cleanup_scan.py asserted removed == 2 but purge_ignored_ips returns total rows deleted across tables`
- 10 min: `tests leaked singleton state (dashboard_cache backend, config, DatabaseManager) across files, making later tests fail (FakeRedis.set(nx=..), no such table, server-IP 204->200)`
- 8 min: `single-process pytest tests/ can hard-crash the interpreter (bus error in aiohttp/frozenlist C extensions) before printing a summary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
