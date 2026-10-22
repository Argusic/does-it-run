# deepseek-php-client

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deepseek-php/deepseek-php-client, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/deepseek-php-client

## Pinned environment

- Project commit: `b02cafe3b4137b8d5b0d9fc182649b4157f573c3`
- Test commit: `b02cafe3b4137b8d5b0d9fc182649b4157f573c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 3 | 4 | 4 | [run](https://argusic.com/run/7fcf8699-7317-448a-a154-f0d1c7761c62) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `php and composer missing in container (no root)`
- 2 min: `e2e run failed with cURL error 7 connection refused because the backgrounded mock server had died when its exec session ended`
- 3 min: `Symfony client sent empty Authorization bearer token; mock's initial lenient auth check returned 200 instead of 401`
- 1 min: `composer test appeared to fail with '/bin/sh: 1: Bad substitution'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
