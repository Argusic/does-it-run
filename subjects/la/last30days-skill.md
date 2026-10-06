# last30days-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mvanhorn/last30days-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/last30days-skill

## Pinned environment

- Project commit: `5103ba478b380552207a3754b74c7655d64208cd`
- Test commit: `5103ba478b380552207a3754b74c7655d64208cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.6 to 35.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34 | 35.6 | 3 | 3 | [run](https://argusic.com/run/293683f9-f9d3-4500-aed8-8a2f006b8b80) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv not found on system PATH`
- 4 min: `System Node v18.19.1 too old: vendored bird-search requires >=22 (import with JSON syntax); caused 2 test failures`
- 1 min: `npx skills package requires Node >= 22.20.0 for crc32 export from node:zlib`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
