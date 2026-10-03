# wizarr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wizarrrr/wizarr, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/wizarr

## Pinned environment

- Project commit: `7bafd55c7c3adbaf9f2d29910db53f5ca02db562`
- Test commit: `7bafd55c7c3adbaf9f2d29910db53f5ca02db562`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.7 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 6.7 | 3 | 3 | [run](https://argusic.com/run/abcbd58e-49e1-4503-a939-281e43f541f0) |
| 2 | pass | 100 | 4 | 10.6 | 1 | 1 | [run](https://argusic.com/run/abf0525c-5208-4d58-bc39-f98640f05af1) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `uv package manager not found on PATH`
- 1.1 min: `Python 3.13+ required but system has Python 3.12`
- 1.5 min: `Database schema missing on first flask run (settings table errors)`

Attempt 2:

- 2 min: `Stale /tmp/wizarr_test.db SQLite WAL/journal artifacts from prior run caused 'disk I/O error' and 'table notification already exists' in test_session_grouping.py and test_invitation_unit.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
