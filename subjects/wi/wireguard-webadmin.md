# wireguard_webadmin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eduardogsilva/wireguard_webadmin, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/wireguard-webadmin

## Pinned environment

- Project commit: `f33cf97753157f108d1acf1cae6bd3789e4a362d`
- Test commit: `f33cf97753157f108d1acf1cae6bd3789e4a362d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.7 to 22.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 22.7 | 11 | 11 | [run](https://argusic.com/run/7560fb43-3676-4e8b-993c-89231bb3a879) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install blocked by PEP 668 externally-managed-environment on Ubuntu 24.04`
- 2 min: `rrdtool-bindings==0.5.0 failed to build: needs Python.h (python3-dev) and librrd headers, unavailable without root`
- 4 min: `wireguard_webadmin/production_settings.py missing (entrypoint.sh normally generates it in Docker)`
- 1 min: `DATABASES path /etc/wireguard/wireguard-webadmin-db.sqlite3 requires root permission`
- 1 min: `STATIC_ROOT /app_static_files/ requires root for collectstatic`
- 4 min: `Django api_v2 tests: test_put_upserts_missing_record_as_create expected 201 without create_if_missing; test_put_upserts_existing_record failed because transaction.on_commit does not fire in TestCase`
- 3 min: `auth-gateway tests failed: caddy/config_files/ directory missing`
- 2 min: `auth-gateway test_invalid_oidc_provider_fails_loudly failed: load_runtime_config did not raise ValueError for invalid OIDC provider URL`
- 1 min: `senha-totp policy required_factors order mismatch: got [password,totp], test expected [totp,password]`
- `ip command not found (iproute2 not installed in container)`
- 1 min: `python manage.py export_configs failed: /etc/wireguard requires root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
