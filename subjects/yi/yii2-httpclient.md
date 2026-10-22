# yii2-httpclient

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yiisoft/yii2-httpclient, licensed BSD-3-Clause, written in PHP.

Evidence and recordings: https://argusic.com/subject/yii2-httpclient

## Pinned environment

- Project commit: `4f70d14acc7b018d64d3d15a891206c5255d43b1`
- Test commit: `4f70d14acc7b018d64d3d15a891206c5255d43b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 2.8 | 2 | 2 | [run](https://argusic.com/run/0bc85c9c-6f89-4b71-8ad2-fc843b53372c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP 8.3.9 (static build) cannot init OpenSSL keys/CSRs: openssl_pkey_new() fails with 'configuration file routines::no such file'`
- 5 min: `php binary and composer not installed in base container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
