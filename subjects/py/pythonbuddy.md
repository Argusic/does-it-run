# PythonBuddy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ethanchewy/PythonBuddy, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/pythonbuddy

## Pinned environment

- Project commit: `91dfbf106c6896455b98ae10bd29386957ffd918`
- Test commit: `91dfbf106c6896455b98ae10bd29386957ffd918`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.8 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.8 | 9 | 9 | [run](https://argusic.com/run/c8e4b3d3-abc9-4bbd-868c-fe88f581ee2c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `greenlet==0.4.17 fails to build from source (no Python.h)`
- 0.3 min: `typed-ast==1.4.1 fails to build from source`
- 0.2 min: `itsdangerous 2.2.0 auto-resolved, Flask 1.1.2 needs 1.x for 'from itsdangerous import json'`
- 0.2 min: `eventlet 0.31.0 uses distutils (removed in Python 3.12)`
- 0.3 min: `eventlet 0.31.0 TypeError: 'is_timeout' on immutable TimeoutError`
- 0.2 min: `dnspython==1.16.0 uses collections.MutableMapping (removed)`
- 0.3 min: `astroid==2.4.2 imports removed 'imp' module`
- 0.3 min: `pylint==2.6.0 incompatible with astroid>=2.15`
- 0.5 min: `epylint DeprecationWarning on stderr triggers pylint_config check`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
