# wechatpay-php

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wechatpay-apiv3/wechatpay-php, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/wechatpay-php

## Pinned environment

- Project commit: `3c9f5c2b71d181e9c244494f695cf5abb53cadc4`
- Test commit: `3c9f5c2b71d181e9c244494f695cf5abb53cadc4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.8 | 2 | 2 | [run](https://argusic.com/run/f97d7fd2-aa14-4dfe-9514-6f14e31ee3c5) |
| 2 | pass | 100 | 4 | 2 | 2 | 2 | [run](https://argusic.com/run/9fd588fe-8bab-4e5d-9348-006b95d53d3a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP and Composer not pre-installed in container`
- 2 min: `Missing test fixture files (mock RSA keys, certificates, serials)`

Attempt 2:

- 1 min: `PHP not installed in container`
- 1 min: `Composer not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
