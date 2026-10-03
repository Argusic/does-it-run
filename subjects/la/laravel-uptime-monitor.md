# laravel-uptime-monitor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spatie/laravel-uptime-monitor, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/laravel-uptime-monitor

## Pinned environment

- Project commit: `04506831232f13c2f2d01d7ab4ee3e1412283842`
- Test commit: `04506831232f13c2f2d01d7ab4ee3e1412283842`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 36 to 36 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 36 | 6 | 6 | [run](https://argusic.com/run/346ad60d-7d21-4845-abc1-1e4add2197be) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `PHP 8.3 not installed in container`
- 8 min: `ext-intl missing from PHP with pdo_sqlite - gnu-bulk PHP had intl but not pdo_sqlite, common had pdo_sqlite but not intl`
- 3 min: `pdo_sqlite.so had 'undefined symbol: php_pdo_unregister_driver' - ABI mismatch when loaded first`
- 6 min: `Ubuntu PHP binary missing shared libraries (libxml2, libsodium, libargon2, libzip)`
- 3 min: `ext-zip not available and unzip command missing`
- 5 min: `Test server boot sequence failed - php and composer commands not resolvable in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
