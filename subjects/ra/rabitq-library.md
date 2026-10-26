# RaBitQ-Library

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VectorDB-NTU/RaBitQ-Library, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/rabitq-library

## Pinned environment

- Project commit: `90943fd046b2114b69fa4f2aa342d2f2148791c0`
- Test commit: `90943fd046b2114b69fa4f2aa342d2f2148791c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10.8 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 12.3 | 0 | 0 | [run](https://argusic.com/run/248917bc-b423-4513-a755-a39d28cf60fb) |
| 2 | pass | 100 | 10 | 10.8 | 3 | 3 | [run](https://argusic.com/run/78f6072a-225b-41f0-b5c1-8cc078e31bd0) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `externally-managed-environment blocks system pip install`
- 3 min: `source build fails: Could NOT find Python (missing Interpreter Development.Module NumPy)`
- 1 min: `Build fails: pyconfig.h include chain broken (x86_64-linux-gnu/python3.12/pyconfig.h not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
