# php-curl-class

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/php-curl-class/php-curl-class, licensed Unlicense, written in PHP.

Evidence and recordings: https://argusic.com/subject/php-curl-class

## Pinned environment

- Project commit: `5b353d51f13368c5039143c4c355b83e29343d60`
- Test commit: `5b353d51f13368c5039143c4c355b83e29343d60`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 43.1 to 43.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 43.1 | 3 | 3 | [run](https://argusic.com/run/08ef042e-bb1e-4cf3-88e8-60ffaf27d4d0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP runtime not found in container`
- 1 min: `Composer not found`
- 35 min: `4 test failures: CURLPROTO_ALL/CURLAUTH_ANY bitmask constants changed from negative to positive in PHP 8.5 curl`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
