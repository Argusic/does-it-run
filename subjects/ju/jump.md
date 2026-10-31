# jump

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/daledavies/jump, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/jump

## Pinned environment

- Project commit: `3aa5b50fe11646469050dd4e94a554dcd83d132c`
- Test commit: `3aa5b50fe11646469050dd4e94a554dcd83d132c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.4 to 35.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 35.4 | 4 | 4 | [run](https://argusic.com/run/a008bf60-44e3-4a84-a823-4f2a00df073d) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Container has no PHP or composer; README requires PHP>=8.1 and composer install --no-dev in jumpapp`
- 12 min: `PHP 8.3 E_DEPRECATED from phlak/config and dynamic-property warnings corrupted raw HTTP bodies on direct output`
- 8 min: `Background server processes were reaped between tool invocations in this sandbox`
- 5 min: `/api/status requires a Nette CSRF session cookie matching the URL token`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
