# fundus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/flairNLP/fundus, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fundus

## Pinned environment

- Project commit: `c1b86b67501872595dc5cccda3ce1c81d6c6f966`
- Test commit: `c1b86b67501872595dc5cccda3ce1c81d6c6f966`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 3.1 | 1 | 1 | [run](https://argusic.com/run/7be746a8-da97-4a51-a283-0a65447e30dc) |

## What was observed on a clean machine

Attempt 1:

- 0.05 min: `pytest 7.2.2 from dev deps is incompatible with Python 3.12 (DeprecationWarning: ast.Str is deprecated)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
