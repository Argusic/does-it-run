# Ecommerce-Laravel-Bootstrap

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kirilkirkov/Ecommerce-Laravel-Bootstrap, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ecommerce-laravel-bootstrap

## Pinned environment

- Project commit: `0dce5617559b33a8daa2010167e5910a275e8a39`
- Test commit: `0dce5617559b33a8daa2010167e5910a275e8a39`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 19.2 to 46.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 46.4 | 0 | 0 | [run](https://argusic.com/run/1169a44d-4467-4351-ba37-e0cb79b2b0df) |
| 2 | pass | 100 | 18 | 19.2 | 4 | 4 | [run](https://argusic.com/run/9c72b73e-43b4-4581-ae5a-db250c432b79) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `PHP not installed in container (no root access for apt-get)`
- 4 min: `PHP 8.3 incompatible with Laravel 7 , deprecation return types cause fatal errors`
- 3 min: `session_start() called at file level in Controller.php runs during autoload before session middleware, causing 'headers already sent'`
- 2 min: `Feature test returned 500 because in-memory SQLite DB had no tables`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
