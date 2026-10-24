# vicinity

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MinishLab/vicinity, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vicinity

## Pinned environment

- Project commit: `c15ab7d7f6afde73d225ac7b9ff31e9e1fc8fa4c`
- Test commit: `c15ab7d7f6afde73d225ac7b9ff31e9e1fc8fa4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 12.3 | 2 | 2 | [run](https://argusic.com/run/79c47679-e592-4747-b289-f6e615daedca) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `hnswlib failed to build: missing Python.h (python3-dev not installed, no root access). No prebuilt wheels available for cp312 on manylinux.`
- 2 min: `annoy failed to build: same root cause as hnswlib , missing Python.h.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
