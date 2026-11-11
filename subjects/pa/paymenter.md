# Paymenter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Paymenter/Paymenter, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/paymenter

## Pinned environment

- Project commit: `927a49a27599f144e20f6d0ffb5b49bf8db07497`
- Test commit: `927a49a27599f144e20f6d0ffb5b49bf8db07497`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.5 to 19.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 19.1 | 4 | 4 | [run](https://argusic.com/run/242a4b0a-c1ab-421d-9ec2-b16f3f021ddf) |
| 2 | pass | 100 | 7 | 7.5 | 5 | 5 | [run](https://argusic.com/run/dc589646-0ec0-4728-b88b-0d768567a6e7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP 8.3 and Composer not pre-installed in container`
- 4 min: `MariaDB server not available in container`
- 1 min: `Node.js 18 too old for Vite 8 build (requires Node >= 20)`
- 1 min: `Test config referenced DB_PORT 3306 instead of 3307, root user had no TCP password`

Attempt 2:

- 2 min: `PHP and Composer were not installed in the container`
- 1 min: `composer post-autoload-dump script failed (artisan package:discover)`
- 2 min: `Feature tests failed with 'View [auth.login] not found' - theme not registered`
- 1 min: `Checkout tests failed - 'Not available in your currency' due to null default_currency config`
- 1 min: `LockSessionTest failed - 'no such table: users' - missing RefreshDatabase trait`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
