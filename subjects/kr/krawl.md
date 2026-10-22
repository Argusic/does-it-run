# Krawl

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BlessedRebuS/Krawl, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/krawl

## Pinned environment

- Project commit: `5b37247c4950d183f71338ecd07dd6a28d6f4955`
- Test commit: `5b37247c4950d183f71338ecd07dd6a28d6f4955`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 35.6 to 92.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 40 | 35.6 | 5 | 5 | [run](https://argusic.com/run/c7dbdcd7-f777-470c-adaa-af6454afe976) |
| 2 | timeout | none | 28 | 92.2 | 4 | 4 | [run](https://argusic.com/run/3c358ec8-3974-4766-a13a-4e36ef5884c2) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `py-tlsh wheel build failed: missing Python.h (python3-dev not installed, no root); no prebuilt cp312 wheel on PyPI`
- 3 min: `tests/test_map_tiles.py expected old ?key= param, code now emits ?api_key=`
- 2 min: `tests/test_startup_cleanup_scan.py asserted removed == 2 but purge_ignored_ips returns total rows deleted across tables`
- 10 min: `tests leaked singleton state (dashboard_cache backend, config, DatabaseManager) across files, making later tests fail (FakeRedis.set(nx=..), no such table, server-IP 204->200)`
- 8 min: `single-process pytest tests/ can hard-crash the interpreter (bus error in aiohttp/frozenlist C extensions) before printing a summary`

Attempt 2:

- 13 min: `py-tlsh 5.0.0 failed to build: /usr/include/python3.12/Python.h missing (no python3-dev headers in container, no prebuilt wheel on PyPI for cp312)`
- 2 min: `pytest not installed and not in requirements.txt`
- 1 min: `Interpreted python test scripts (test_threat_capture.py etc.) are main()-guarded and pytest reports 'no tests ran'`
- 12 min: `Running all collected tests in one pytest process shows 7 pre-existing failures that are ORM-identity-map pollution between tests (old IpStats objects re-persist into the next test's DB after the prior file was unlinked) plus two spec-vs-co`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
