# diagrams

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mingrammer/diagrams, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/diagrams

## Pinned environment

- Project commit: `0cd0d84016087eead0f7a5b747571b3f92b56726`
- Test commit: `0cd0d84016087eead0f7a5b747571b3f92b56726`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.3 | 3 | 3 | [run](https://argusic.com/run/cb62943f-1cde-48ff-a567-4ef6a16f948a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 prevents global pip installs (Ubuntu 24.04)`
- 1 min: `Graphviz system binary not installed`
- 0.5 min: `pytest not installed in the environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
