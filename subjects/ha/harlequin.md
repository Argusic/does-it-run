# harlequin

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tconbeer/harlequin, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/harlequin

## Pinned environment

- Project commit: `5c463bf8b29e5d25f466ab48680b7c1bfb28e7a7`
- Test commit: `5c463bf8b29e5d25f466ab48680b7c1bfb28e7a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 41.1 to 78.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 78.9 | 0 | 0 | [run](https://argusic.com/run/e3023990-1766-48a3-be23-5a2031bd6c3e) |
| 2 | pass | 100 | 2 | 41.1 | 1 | 1 | [run](https://argusic.com/run/b8dbc5e3-54a9-4eb5-b0e9-7e5eaf3cbce7) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Locale en_US.UTF-8 not available in minimal container (only C/C.utf8/POSIX installed). Tests errored at setup with HarlequinLocaleError.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
