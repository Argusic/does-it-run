# http

**Verdict: runs.** Argusic Score 65 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reactphp/http, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/run/c44315a3-014c-4509-b914-16f3e174e873

## Pinned environment

- Project commit: `bb151a7cdf9e7b49caac9030add52c6427ebc6d2`
- Test commit: `bb151a7cdf9e7b49caac9030add52c6427ebc6d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 2.8 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 0.1 | 7.3 | 1 | 0 | [run](https://argusic.com/run/c44315a3-014c-4509-b914-16f3e174e873) |
| 2 | pass | 100 | 2 | 2.8 | 4 | 4 | [run](https://argusic.com/run/7d36eb80-4b81-4ebb-a430-436bf277fa48) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `selftest output missing`

Attempt 2:

- 1 min: `PHP interpreter not found on system`
- 1 min: `Composer not found on system`
- `Default memory_limit 128M insufficient for MultipartParserTest; test exhausted memory (tried to allocate 535MB)`
- `SSL certificate verify failed connecting to www.google.com:443 , static PHP lacks default openssl.cafile`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
