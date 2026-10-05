# evennia

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/evennia/evennia, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/evennia

## Pinned environment

- Project commit: `a89a9b94e4d7ed0acfee86def533b77bf6baa512`
- Test commit: `a89a9b94e4d7ed0acfee86def533b77bf6baa512`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 36.5 to 95.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 2 | 95.3 | 3 | 3 | [run](https://argusic.com/run/37365c5a-afa1-464e-9054-c437bd99c94d) |
| 2 | pass | 100 | 8 | 36.5 | 0 | 0 | [run](https://argusic.com/run/e2d361bc-1497-455f-93a2-bb6efd636df6) |

## What was observed on a clean machine

Attempt 1:

- `Migration 0017 uses get_operations() pattern never called by Django 5.1+`
- `EvenniaLogFile accesses settings at class definition time`
- `Twisted reactor conflicts when running multiple test modules in one process`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
