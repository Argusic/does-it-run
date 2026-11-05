# Sylius

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sylius/Sylius, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/sylius

## Pinned environment

- Project commit: `38588aff004e9ad66fe78e3c8b61791709b57659`
- Test commit: `38588aff004e9ad66fe78e3c8b61791709b57659`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 23.8 to 42.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 23.8 | 3 | 3 | [run](https://argusic.com/run/45dadb57-5d9e-4f8f-8221-33e9accab981) |
| 2 | pass | 100 | 32 | 42.6 | 5 | 5 | [run](https://argusic.com/run/3cd1e5ae-7b88-4bc3-87a3-aa5148d436da) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP not pre-installed in container. composer required php.`
- 1 min: `composer post-install cache:clear failed: Allowed memory size of 134217728 bytes exhausted`
- 2 min: `cache:clear failed: SQLSTATE[HY000] [2002] Connection refused (MySQL not available)`

Attempt 2:

- 18 min: `PHP 8.3, Composer, MySQL and Yarn were not present in the container and no apt/root was available; the README stack expects php 8.3 Docker image + MySQL`
- 4 min: `sylius:install on a pre-created empty DB rolled back leaving no sylius_currency table; also first run hit No such file session.save_path (/var/lib/php/sessions)`
- 6 min: `yarn install and yarn encore failed with engine error node>=22 vs node 18.19.1 (package.json engines, engineStrict)`
- 0.5 min: `phpstan analyse failed: PHPDoc @var DateTimeInterface not subtype of native DateTimeImmutable in ProductLowestPriceBeforeDiscountProcessor.php:83`
- 6 min: `vendor/bin/ecs (EasyCodingStandard 13.1.2) fatals at startup under PHP 8.3: bundled squizlabs/php_codesniffer Tokens.php references T_AND_EQUAL/T_POW/T_COMMENT etc. that are undefined at class load, and the parallel worker also fails; --no-`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
