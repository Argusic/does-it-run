# laravel-seo-scanner

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/backstagephp/laravel-seo-scanner, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/laravel-seo-scanner

## Pinned environment

- Project commit: `6a3b55056708669aa34b2d8f82819a8787e1cb6f`
- Test commit: `6a3b55056708669aa34b2d8f82819a8787e1cb6f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.9 to 27.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 27.9 | 5 | 5 | [run](https://argusic.com/run/1aada610-cb92-40c1-8770-91fa1ad7ace6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No php/composer in container (no root): used prebuilt static PHP 8.4.23 + Composer 2.10.3 to install 138 packages`
- 1 min: `composer test failed with /usr/bin/env: php: No such file or directory`
- 1 min: `composer analyse failed: PHPStan worker hit 128M memory limit`
- 3 min: `Real seo:scan-url returned empty checks (score 0, 0 checks): config check_paths pointed to base_path('vendor/backstage/laravel-seo-scanner/src/Checks') which does not exist in this dev-copy install`
- 1 min: `seo:scan with database.save=true failed: Table 'seo_test.seo_scans' doesn't exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
