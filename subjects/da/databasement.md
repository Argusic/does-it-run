# databasement

**Verdict: runs.** Argusic Score 98.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/David-Crty/databasement, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/databasement

## Pinned environment

- Project commit: `a11dd82e08553af61b8249264a96fe461a3c4e75`
- Test commit: `a11dd82e08553af61b8249264a96fe461a3c4e75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 64.5 to 65.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 50 | 64.5 | 5 | 5 | [run](https://argusic.com/run/cf044ae4-ca3d-423e-99f7-a73d8be60f13) |
| 2 | pass | 96.67 | 30 | 65.7 | 6 | 5 | [run](https://argusic.com/run/3ddf2366-be6b-404a-9b41-d81dc1a75604) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `PHP 8.5 runtime and extensions not pre-installed`
- 5 min: `ext-mongodb not available in PPA: no PHP MongoDB driver packages exist`
- 5 min: `libzip.so.4 missing from system, preventing zip extension loading`
- 10 min: `pdo_mysql/mysqli extensions depend on mysqlnd which is compiled into CLI (not a separate .so) , pdo_mysql cannot load because mysqlnd symbols resolve from the wrong extension boundary`
- 2 min: `ext-xmlwriter required libxml2 available system-wide but was not in php.ini`

Attempt 2:

- 10 min: `No PHP, Composer, or Docker in container (no root) - nothing could build or run`
- 15 min: `composer install failed: ext-mongodb missing (no PECL build for static PHP)`
- 5 min: `npm run build failed: Node 18 too old for Vite 8 (CustomEvent undefined), and native rolldown binding missing after --ignore-scripts`
- 10 min: `A composer update that bumped laravel/framework v13.24.0->v13.42.0 regressed cross-organization scope tests (ModelNotFoundException not thrown)`
- 5 min: `Feature test DatabaseServer\CreateTest expects Docker-image path /opt/mysql-client/bin/mysqldump which does not exist outside the Docker image`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
