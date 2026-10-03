# laravel-backup

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spatie/laravel-backup, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/laravel-backup

## Pinned environment

- Project commit: `2b39b6b0fb98eefb95f1ef6b6311983396823c72`
- Test commit: `2b39b6b0fb98eefb95f1ef6b6311983396823c72`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.8 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13.8 | 2 | 2 | [run](https://argusic.com/run/a799fd99-0ebb-4a57-b578-c5971c9a7425) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP binary not found in container (no php, no composer, no apt)`
- 2 min: `sqlite3 CLI not found, causing all --only-db backup tests to fail (21 failures)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
