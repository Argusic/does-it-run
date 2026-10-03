# bagisto

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bagisto/bagisto, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/bagisto

## Pinned environment

- Project commit: `805b67013134ebc53f1da1285f0aa6632f5dde62`
- Test commit: `805b67013134ebc53f1da1285f0aa6632f5dde62`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31.6 to 31.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 27 | 31.6 | 4 | 4 | [run](https://argusic.com/run/ea64aca2-336b-4dbd-aa8e-944515cf072b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP 8.3+ not installed in container`
- 1 min: `Composer not installed`
- 5 min: `No MySQL or Redis available; no apt-get access (no root)`
- 3 min: `Database seeder CategoryTableSeeder inserts root category translation without url_path (NOT NULL column)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
