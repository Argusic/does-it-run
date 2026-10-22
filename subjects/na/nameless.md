# Nameless

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NamelessMC/Nameless, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/nameless

## Pinned environment

- Project commit: `298a2e7a5acae005c12f0d82dee62bddcadc9d17`
- Test commit: `298a2e7a5acae005c12f0d82dee62bddcadc9d17`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29 to 29 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 29 | 3 | 3 | [run](https://argusic.com/run/aedcb61a-f86d-4761-bf91-2f8d04bf9d7a) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `PHP 8.2+, MariaDB and nginx were not installed in the container and could not be installed via apt (no root)`
- 3 min: `php ext gd.so/zip.so/xsl.so failed to load: missing system libgd/libzip/libxslt`
- 3 min: `Every HTTP request logged session_start(): Failed to read session data (files: /var/lib/php/sessions) and POST login always returned 'Invalid token, please try again.' because php-fpm default session.save_path was unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
