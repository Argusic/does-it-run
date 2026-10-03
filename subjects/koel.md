# koel

**Verdict: runs.** Argusic Score 98.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/koel/koel, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/koel

## Pinned environment

- Project commit: `41cab99feeaf59b139699403fdfd41f0a280fb39`
- Test commit: `41cab99feeaf59b139699403fdfd41f0a280fb39`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 21.1 to 27.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 27.5 | 5 | 5 | [run](https://argusic.com/run/04bd2166-4d92-48db-9054-85a4f00ffaad) |
| 2 | pass | 100 | 8 | 21.1 | 5 | 5 | [run](https://argusic.com/run/4e35a205-c7f6-4d80-b99c-66b60219b6b3) |
| 3 | pass | 96.36 | 45.1 | 26.9 | 11 | 9 | [run](https://argusic.com/run/7a4e4bf2-0dec-44c2-bddf-68fc91b613b3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP not installed in container (no apt install possible without root)`
- 1 min: `Missing PHP extensions ext-intl, ext-xsl, ext-sodium in common PHP build (needed by composer deps)`
- 1 min: `Node.js v18 too old (project requires >=20.19.0)`
- 1 min: `pnpm could not be installed globally (EACCES)`
- 1 min: `SQLite database path misconfigured in .env`

Attempt 2:

- 6 min: `PHP 8.4+/composer not installed in container`
- 1 min: `Artisan package:discover failed on post-install , no .env configured for SQLite`
- 1 min: `PDO::MYSQL_ATTR_SSL_CA deprecated in PHP 8.5 in config/database.php`
- 5 min: `Node.js v18 too old; vite-plus requires Node 22+ for styleText from node:util`
- 2 min: `php artisan serve not supported by frankenphp wrapper`

Attempt 3:

- 1 min: `PHP 8.x binary not present in container`
- 0.5 min: `Composer binary not present in container`
- 3 min: `pnpm binary not present and npm install -g failed (EACCES)`
- 3 min: `Node.js v18 lacked styleText from node:util needed by vite-plus`
- 1 min: `Missing PHP extensions: ext-intl, ext-xsl, ext-sodium (not in static build)`
- 2 min: `pnpm install failed on initial run: vite-plus prepare script crashed under Node v18`
- 0.5 min: `koel:init --no-assets failed: crontab not available for scheduler install`
- 15 min: `php artisan serve returned 500 on first request (Vite manifest missing)`
- 2 min: `Login endpoint rejected default password (admin created without seed)`
- `Frontend vitest tests hang with vp test runner`
- `Frontend vitest tests also hang with npx vitest (reporter loading error)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
