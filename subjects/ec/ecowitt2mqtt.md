# ecowitt2mqtt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bachya/ecowitt2mqtt, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ecowitt2mqtt

## Pinned environment

- Project commit: `552afdf06df10ccff5b4e3c940b00d423d050b70`
- Test commit: `552afdf06df10ccff5b4e3c940b00d423d050b70`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5 | 2 | 2 | [run](https://argusic.com/run/ccc099a8-6dd8-4bca-85ae-d56791ce208d) |

## What was observed on a clean machine

Attempt 1:

- `multidict 6.0.4 has no binary wheel for Python 3.12; build from source fails because python3-dev headers are missing (no root access)`
- 1 min: `locale 'en_US.UTF-8' is not available in this container (only C.UTF-8)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
