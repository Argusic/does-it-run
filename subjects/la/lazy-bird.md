# lazy-bird

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yusufkaraaslan/lazy-bird, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/lazy-bird

## Pinned environment

- Project commit: `a9bbc35cb2dc571d787384e12828eb1b3adf602c`
- Test commit: `a9bbc35cb2dc571d787384e12828eb1b3adf602c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 9.7 | 6 | 6 | [run](https://argusic.com/run/2e0b7e5c-390a-4aaf-b7b1-a2f3abd33f56) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Import of lazy_bird failed: SQLAlchemy async requires 'greenlet' which was not declared in requirements`
- 2 min: `lazy_bird/core/database.py uses the 'psycopg' (v3) dialect but only psycopg2-binary was declared, causing ModuleNotFoundError: No module named 'psycopg'`
- 2 min: `Async engine creation failed: ModuleNotFoundError: No module named 'asyncpg'`
- 4 min: `Flask web backend crashed on startup: PermissionError creating /var/lib/lazy_birtd/queue (not writable without root)`
- 1 min: `Flask web backend: No module named 'github' (PyGithub) - web/backend/requirements.txt was never installed`
- 1 min: `tests/security/test_security_audit.py failed: my hand-created ~/.config/lazy_birtd/secrets had mode 775 instead of required 700`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
