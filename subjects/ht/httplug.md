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
- Valid runs: 2; wall time 2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.2 | 3 | 3 | [run](https://argusic.com/run/bcdefba0-b923-4ea7-b785-99e791d9a7be) |
| 2 | pass | 100 | 5 | 2 | 5 | 5 | [run](https://argusic.com/run/999f4f98-cb4e-4ec1-b2ff-1fca2a4283c6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP runtime not installed in container`
- 2 min: `PHP 8.4 incompatible with phpspec 7.6.0 (E_DEPRECATED breaks 34 tests)`
- 1 min: `PHP 8.2 incompatible with sebastian/comparator (OVERLONG_THRESHOLD parse error)`

Attempt 2:

- 2 min: `PHP not installed in container`
- 1 min: `Composer not installed`
- 1 min: `PHP 8.4 too new for dependency constraints; phpspec/phpspec requires PHP ^7.1 || ^8.0.* || ^8.1.* || ^8.2.* || ^8.3.*`
- 1 min: `Existing lock file was generated with PHP 8.4 and contained packages requiring ^8.4`
- 1 min: `Tests produced 34 broken examples with PHP 8.4 due to E_DEPRECATED errors in phpspec`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
