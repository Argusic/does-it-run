# AstrLink

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Calcium-Ion/AstrLink, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/astrlink

## Pinned environment

- Project commit: `3779884c67d9d7acd9ab921430ae885d906affed`
- Test commit: `3779884c67d9d7acd9ab921430ae885d906affed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 17.8 | 5 | 5 | [run](https://argusic.com/run/5c171a78-cdd2-4def-bf5c-b8ab10022007) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Bun requires unzip which was not installed`
- 2 min: `Go not found`
- `Ruby not found for contracts/validate.rb`
- `Desktop Tauri needs glib-2.0 system library`
- 2 min: `Core dies when stdin pipe closes after reading start tokens`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
