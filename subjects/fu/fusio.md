# fusio

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apioo/fusio, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/fusio

## Pinned environment

- Project commit: `4acff95ad952d6677b887e939d87b7ad1cf72b56`
- Test commit: `4acff95ad952d6677b887e939d87b7ad1cf72b56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.4 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 7.4 | 0 | 0 | [run](https://argusic.com/run/ea77d7ff-32c9-4cab-8b32-a9ed690847aa) |
| 2 | pass | 100 | 18 | 17.5 | 5 | 5 | [run](https://argusic.com/run/0407be27-701d-4add-8a52-4a43d2bf4ef9) |

## What was observed on a clean machine

Attempt 2:

- 6 min: `No PHP binary available in container`
- 3 min: `Missing PHP extensions (curl, mbstring, pdo, soap, sqlite, etc.)`
- 2 min: `Composer lock requires PHP >= 8.4 but only PHP 8.3 available via apt`
- 1 min: `Missing unzip tool for composer install`
- 1 min: `SQLite database path wrong in .env (pdo-sqlite:/// requires 3 slashes for absolute path)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
