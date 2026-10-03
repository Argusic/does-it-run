# yii2_fecshop

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fecshop/yii2_fecshop, licensed BSD-3-Clause, written in PHP.

Evidence and recordings: https://argusic.com/subject/yii2-fecshop

## Pinned environment

- Project commit: `19c5cb8f4848a6ef0194e3b9add050c5853cae94`
- Test commit: `19c5cb8f4848a6ef0194e3b9add050c5853cae94`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 15.4 to 25 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 15.4 | 6 | 6 | [run](https://argusic.com/run/7319c95f-7688-4912-81c4-3a074f406cb4) |
| 2 | fail | 20 | n/a | 25 | 0 | 0 | [run](https://argusic.com/run/e0c8e862-6710-4464-b39d-ad87d2bbde0a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP and composer not installed in container`
- 1 min: `composer.json missing asset-packagist repository for bower-asset dependencies`
- 1 min: `league/iso3166 ^2.1 incompatible with PHP 8.2`
- 1 min: `geoip2/geoip2 2.10.0 incompatible with PHP 8.2`
- 1 min: `phpoffice/phpexcel blocked by security advisory`
- 1 min: `yii/Yii.php had wrong relative path for BaseYii.php`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
