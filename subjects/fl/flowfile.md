# Flowfile

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Edwardvaneechoud/Flowfile, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/flowfile

## Pinned environment

- Project commit: `ec12885c61af605f907e07bbbc59aaeb51a7986a`
- Test commit: `ec12885c61af605f907e07bbbc59aaeb51a7986a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 31 | 1 | 1 | [run](https://argusic.com/run/cc853f51-48f7-497b-83ac-ce80dd924e6f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `find_parent_directory('Flowfile') fails when repo root directory is not named 'Flowfile'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
