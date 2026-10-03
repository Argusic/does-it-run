# docs

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/suitenumerique/docs, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/docs

## Pinned environment

- Project commit: `5b24290923e517e314971c13fdb58c09311fd223`
- Test commit: `5b24290923e517e314971c13fdb58c09311fd223`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 42 to 78.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/7bff1f9a-0808-4428-b65b-e5bdc1313bda) |
| 1 | fail | 80 | 88 | 78.9 | 8 | 8 | [run](https://argusic.com/run/6607d875-df8c-4cbc-a9ad-d12ef6c8a428) |
| 2 | pass with mocks | 92 | 54 | 62.3 | 9 | 9 | [run](https://argusic.com/run/6bccdf0a-1f39-47b4-adb2-d3b7f9f8f40c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Python 3.12 default too old; installed Python 3.14 via uv`
- 10 min: `libmagic system library not installed (no root)`
- 20 min: `PostgreSQL not installed and cannot install without root`
- 15 min: `Django treebeard model uses db_collation='C' only supported on PostgreSQL`
- 15 min: `Django ArrayField generates varchar(255)[] type valid only on PostgreSQL`
- 8 min: `S3/MinIO not available for S3-dependent storage tests`
- 5 min: `mozilla_django_oidc requires OIDC_OP_JWKS_ENDPOINT or key`
- 10 min: `uv pip install was very slow on fresh venv`

Attempt 2:

- 1 min: `Python 3.12 incompatible with pyproject.toml requires-python='~=3.14.0'`
- 2 min: `Syntax errors: 6 files used 'except E1, E2:' (Python 3.11+ requirement) which fails in Python 3.12`
- 5 min: `PostgreSQL not installed in container`
- 2 min: `No Redis available for cache/celery`
- 3 min: `libmagic (python-magic dependency) not found`
- 3 min: `S3 credentials required for MinIO (Default storage uses S3)`
- 1 min: `itertools.batched() took 'strict' keyword arg (Python 3.13+ only)`
- 2 min: `Email templates missing (MJML not compiled)`
- 2 min: `Locale .mo files missing (only .po files present)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
