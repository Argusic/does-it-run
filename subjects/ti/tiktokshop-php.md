# tiktokshop-php

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EcomPHP/tiktokshop-php, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/tiktokshop-php

## Pinned environment

- Project commit: `fbeedcaf2a3ecb2a2665b2abfe7e8ed17f322b4c`
- Test commit: `fbeedcaf2a3ecb2a2665b2abfe7e8ed17f322b4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.5 to 1.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 1.5 | 2 | 2 | [run](https://argusic.com/run/50ac9eb8-90dc-49e8-835a-f11e9861a07b) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `php and composer not installed in container`
- 1 min: `vendor/bin/phpunit shebang failed: /usr/bin/env: php: No such file or directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
