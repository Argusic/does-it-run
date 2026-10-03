# BookStack

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BookStackApp/BookStack, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/bookstack

## Pinned environment

- Project commit: `1633b3ab281b2df34a1c03e9370a2b756ba4d894`
- Test commit: `1633b3ab281b2df34a1c03e9370a2b756ba4d894`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 32.8 to 32.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 31 | 32.8 | 6 | 6 | [run](https://argusic.com/run/ccefd565-d911-4326-8a0c-faa5f62f384b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP and Composer not installed`
- 3 min: `No MySQL database server available`
- 1 min: `Migration macro 'indexed()' undefined in Laravel 12`
- 1 min: `LDAP tests fail (7 errors, 22 failures) - PHP ext-ldap not loaded`
- 1 min: `PDF export test failure - php not in PATH for subprocess`
- 1 min: `Config tests fail - STORAGE_TYPE=local_secure not supported and MySQL port mismatch 3307 vs 3306`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
