# pandas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pandas-dev/pandas, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/pandas

## Pinned environment

- Project commit: `63651d6717faa0fb850c2723c0183194255d6e1c`
- Test commit: `63651d6717faa0fb850c2723c0183194255d6e1c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 15.1 | 6 | 6 | [run](https://argusic.com/run/e98edd8e-df57-42f0-bb5d-c0781e0af861) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `externally-managed-environment blocked pip installs (PEP 668)`
- 0.5 min: `Could not find ninja version 1.8.2 or newer`
- 8 min: `Cython requires python3 dependency for link testing - missing Python.h and libpython3.12`
- 1 min: `fatal error: x86_64-linux-gnu/python3.12/pyconfig.h not found`
- 2 min: `cannot find -lpython3.12 / libpython3.12.a cannot make shared object`
- 0.5 min: `ZoneInfoNotFoundError 'No time zone found with key US/Pacific' (tzdata-legacy missing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
