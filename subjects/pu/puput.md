# puput

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/APSL/puput, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/puput

## Pinned environment

- Project commit: `ce7a2f5293c4778f144e16ba9cd5e8ce1c348f27`
- Test commit: `ce7a2f5293c4778f144e16ba9cd5e8ce1c348f27`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 11.1 | 3 | 3 | [run](https://argusic.com/run/792ab2de-06ab-46db-b1ac-d3f50b4da914) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pytest-django: No module named 'tests' , PYTHONPATH not set`
- 20 min: `Committed tests/testapp/puput.db is an old Wagtail/SQLite schema; live GETs hit 'no such column translation_key' and entry creation hit 'NoneType _inc_path' and Document DoesNotExist`
- 1 min: `auth_user UNIQUE constraint during live entry-creation scripting (legacy admin row present)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
