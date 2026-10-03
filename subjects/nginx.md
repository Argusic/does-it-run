# nginx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nginx/nginx, licensed BSD-2-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/nginx

## Pinned environment

- Project commit: `939334efff3575ce52597cc8c13d55821044ac57`
- Test commit: `939334efff3575ce52597cc8c13d55821044ac57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 5.1 | 3 | 3 | [run](https://argusic.com/run/29fab5b7-4447-41fb-b116-67e596631221) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `configure failed: PCRE library not found (no libpcre3-dev, no root)`
- 1 min: `configure would have failed for zlib (no zlib1g-dev, no root)`
- 1 min: `nginx -t failed: cannot open conf/logs under /usr/local/nginx/ (no write permission)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
