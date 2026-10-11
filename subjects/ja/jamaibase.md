# JamAIBase

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EmbeddedLLM/JamAIBase, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/jamaibase

## Pinned environment

- Project commit: `56ffb4653ff263ecfa09c7562daa1710febb221e`
- Test commit: `56ffb4653ff263ecfa09c7562daa1710febb221e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 14.7 to 33.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 60 | 9 | 14.7 | 2 | 0 | [run](https://argusic.com/run/6b3e2ad7-b847-4671-b041-2cf362f271cf) |
| 2 | pass | 100 | 31 | 33.5 | 3 | 3 | [run](https://argusic.com/run/5d72f623-75a0-4a28-b079-e0c27f228401) |

## What was observed on a clean machine

Attempt 1:

- `PostgreSQL not available , the API server and its DB-backed tests require a PostgreSQL 17 instance, which cannot be installed (no root). The config validation also blocks SQLite fallback even though SQLAlchemy + aiosqlite are present.`
- `test_auth.py::test_has_permissions has a pre-existing failure: pytest.raises(ValueError) is not raised because the has_permissions function no longer raises ValueError when both org/proj IDs are missing (the test is also marked @pytest.mark`

Attempt 2:

- 1 min: `externally-managed-environment prevents system pip install`
- 4 min: `No PostgreSQL server installed in container`
- 6 min: `No Redis server available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
