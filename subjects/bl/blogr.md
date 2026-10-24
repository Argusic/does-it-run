# blogr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bahdotsh/blogr, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/blogr

## Pinned environment

- Project commit: `46bf0f9faa1214dcd60ced372ea4c6666dba8110`
- Test commit: `46bf0f9faa1214dcd60ced372ea4c6666dba8110`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 7.2 | 1 | 1 | [run](https://argusic.com/run/a4bf491e-b60b-4ca3-8947-c17c729d1227) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `blogr serve with auto_reload=true fails: 'Too many open files (os error 24)' from notify/inotify`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
