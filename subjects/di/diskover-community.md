# diskover-community

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/diskoverdata/diskover-community, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/diskover-community

## Pinned environment

- Project commit: `c2ba335880e96fc26300db496ee69193ad349678`
- Test commit: `c2ba335880e96fc26300db496ee69193ad349678`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 17.6 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 17.6 | 5 | 5 | [run](https://argusic.com/run/1d6835c4-f8a5-4f07-a098-8e3e92144a1d) |
| 2 | pass | 100 | 21 | 23 | 5 | 5 | [run](https://argusic.com/run/d43806a8-1ee1-4928-a5f0-30b8798a8fd8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Elasticsearch (Java) available for real connection - needed PHP 8+, Nginx, and Elasticsearch 8.x for full stack`
- 1 min: `Python externally-managed environment prevented pip install system-wide`
- 1 min: `SQLite database default path (/var/www/diskover-web/) not writable`
- 3 min: `SyntaxWarning on escape sequences in banner() string`
- `PHP 8+, Nginx not installed - web frontend cannot launch`

Attempt 2:

- 2 min: `PEP 668 externally-managed-environment blocks system-wide pip install`
- 6 min: `Elasticsearch 7.13.1 default heap (3.7GB) exceeds container memory (773MB); process OOM-killed`
- 8 min: `Elasticsearch daemon failed silently due to stale pid file from prior run`
- 1 min: `Python scanner failed with 'unable to open database file' because DATABASE path defaults to /var/www/diskover-web/diskoverdb.sqlite3 which does not exist`
- 3 min: `No PHP or Nginx packages available (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
