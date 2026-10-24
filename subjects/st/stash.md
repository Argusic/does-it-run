# stash

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fergana-Labs/stash, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/stash

## Pinned environment

- Project commit: `57ec4b0549738a4997062c6e85394c7e6b734139`
- Test commit: `57ec4b0549738a4997062c6e85394c7e6b734139`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.1 to 24.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 24.1 | 2 | 2 | [run](https://argusic.com/run/ad519f75-4821-4ecb-b7ca-da5b7a7565cc) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `PostgreSQL 16 not installed; required for backend tests`
- 5 min: `Node 18 too old for frontend (vitest/rolldown need Node 22)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
