# redd-archiver

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/19-84/redd-archiver, licensed Unlicense, written in Python.

Evidence and recordings: https://argusic.com/subject/redd-archiver

## Pinned environment

- Project commit: `bd4018311a1404194689ca0dc1d763f3125eb871`
- Test commit: `bd4018311a1404194689ca0dc1d763f3125eb871`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.2 | 1 | 1 | [run](https://argusic.com/run/32d6aa4a-489b-4af6-b23e-35593ceba41b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PostgreSQL 16 not installed and no root access for apt install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
