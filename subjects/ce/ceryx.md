# ceryx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/withlogicco/ceryx, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ceryx

## Pinned environment

- Project commit: `6b642b72dcce8ad8a29927c8dff84d88b6520cd4`
- Test commit: `6b642b72dcce8ad8a29927c8dff84d88b6520cd4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 23.3 to 26.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 26.1 | 5 | 5 | [run](https://argusic.com/run/ce20a2a1-d440-4578-b14e-121e513d0003) |
| 2 | pass | 100 | 30 | 23.3 | 5 | 5 | [run](https://argusic.com/run/b11d8793-ec90-4874-81d9-e7473a57f728) |

## What was observed on a clean machine

Attempt 1:

- `nginx and dockerize not present in container; Lua module not available`
- `tests/utils.py create_certificates_for_host fails on re-run because openssl cannot overwrite chmod 444 files`
- `tests/utils.py CERTIFICATE_ROOT hardcoded to /usr/local/share/certificates (not writable)`
- `tests/test_certificates.py uses hardcoded /etc/ceryx/ssl/default.crt for SSL verification`
- `tests/test_mtls.py uses hardcoded /usr/local/share/certificates path`

Attempt 2:

- 10 min: `nginx and related packages not pre-installed in container (no root access)`
- 8 min: `Missing resty.redis, resty.openssl.*, resty.auto-ssl Lua modules`
- 7 min: `Hardcoded system paths (/usr/local/share/certificates, /etc/ceryx/ssl) in tests and templates`
- 2 min: `DNS resolver (8.8.8.8) couldn't resolve local hostnames`
- 3 min: `CERYX_TLS_DEFAULT_CERTIFICATE env var overrode CERYX_SSL_DEFAULT_* in Go template chain`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
