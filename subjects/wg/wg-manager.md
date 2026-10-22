# wg-manager

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/perara/wg-manager, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/wg-manager

## Pinned environment

- Project commit: `e70ba4bdc288318bc164fe696750a0c40ed1fac6`
- Test commit: `e70ba4bdc288318bc164fe696750a0c40ed1fac6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.5 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 16.5 | 9 | 9 | [run](https://argusic.com/run/e65797ea-62cc-4ccc-8019-4289740193bd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pydantic v2 removed pydantic.typing.List and GenericModel (import of main crashed)`
- 1 min: `pkg_resources missing on Python 3.12 (ModuleNotFoundError)`
- 2 min: `database/__init__.py empty so tests could not import SessionLocal`
- 3 min: `tests hit non-existent /api/* paths and wrong login content type (5 failures)`
- 2 min: `passlib 1.7.4 crashed against bcrypt>=4.1 (ValueError 72 bytes)`
- 3 min: `starting server from repo root failed: relative alembic.ini/migrations and build/ paths`
- 3 min: `angular build failed on Node 18 (ERR_OSSL_EVP_UNSUPPORTED) and npm peer conflict`
- 5 min: `wg endpoints return 500 (FileNotFoundError: 'wg'); wireguard-tools not installed in container and no root to apt install`
- 1 min: `npm peer conflict angular-material-dynamic-themes requires old @angular/material`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
