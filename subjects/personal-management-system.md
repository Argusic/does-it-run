# personal-management-system

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Volmarg/personal-management-system, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/personal-management-system

## Pinned environment

- Project commit: `c138c6db98b184cdda5e584b5bcca7bd1c377a02`
- Test commit: `c138c6db98b184cdda5e584b5bcca7bd1c377a02`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 16.4 to 25.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 25.2 | 5 | 5 | [run](https://argusic.com/run/3673d1cd-492a-48ec-807e-4c9859b0c481) |
| 2 | pass with mocks | 92 | 15 | 16.4 | 6 | 6 | [run](https://argusic.com/run/fe81fef2-6677-4a77-bb63-5118e24a9bbe) |
| 3 | pass | 100 | 18 | 17.5 | 9 | 9 | [run](https://argusic.com/run/bc71863b-b4ca-4bfd-a9c5-7b0e5ac3205f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP not installed in container`
- 1 min: `composer.lock requires PHP ^7 for dev dependencies (paragonie/random_compat, phpunit)`
- 8 min: `No MySQL/MariaDB database server available`
- 1 min: `Upload/PROFILE_IMAGE directory missing (causes 500 on login success handler)`
- 2 min: `MariaDB required --innodb-buffer-pool-size=8M and --skip-grant-tables to run in constrained environment`

Attempt 2:

- 5 min: `PHP not installed in container (no php binary)`
- 1 min: `Composer 2.1.3 phar emits deprecation warnings on PHP 8.5`
- 1 min: `Missing symfony/twig-bundle in installed packages`
- 1 min: `Environment variable APP_IPS_ACCESS_RESTRICTION not set, causing 500 errors`
- 2 min: `No MySQL/MariaDB server available; project requires MySQL for full functionality`
- `No phpunit.xml or test files exist in tests/ directory`

Attempt 3:

- 2 min: `PHP not available in the container`
- 1 min: `composer.lock packages require PHP ^7.x (various dev packages) and ext-sodium`
- 1 min: `symfony/twig-bundle was not installed despite being in bundles.php`
- 1 min: `Doctrine cache configured for APCu which is not available`
- 6 min: `MariaDB not installed, no Docker available`
- 2 min: `MariaDB client missing libncurses.so.6`
- 1 min: `Doctrine entities use ENUM() column definitions incompatible with SQLite`
- 1 min: `Missing upload/PROFILE_IMAGE directory causes login crash`
- 1 min: `Login uses 'username' key not 'email' despite user_identity_field: email in config`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
