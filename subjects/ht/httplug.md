# httplug

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/php-http/httplug, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/httplug

## Pinned environment

- Project commit: `37819ce3c78ed2e7d001de68b38e697bbd525f89`
- Test commit: `37819ce3c78ed2e7d001de68b38e697bbd525f89`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.2 | 3 | 3 | [run](https://argusic.com/run/bcdefba0-b923-4ea7-b785-99e791d9a7be) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP runtime not installed in container`
- 2 min: `PHP 8.4 incompatible with phpspec 7.6.0 (E_DEPRECATED breaks 34 tests)`
- 1 min: `PHP 8.2 incompatible with sebastian/comparator (OVERLONG_THRESHOLD parse error)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
