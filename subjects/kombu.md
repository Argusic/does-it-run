# kombu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/celery/kombu, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/kombu

## Pinned environment

- Project commit: `82577320de2ee6c5af0b8c6fc234d44bacfc1010`
- Test commit: `82577320de2ee6c5af0b8c6fc234d44bacfc1010`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 5.5 | 5 | 5 | [run](https://argusic.com/run/a96ffcaa-8a84-492a-b63c-c7f85b9c69d8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally-managed environment blocks pip install`
- 1 min: `ModuleNotFoundError: No module named 'botocore'`
- 2 min: `ModuleNotFoundError: No module named 'azure' in test_azurestoragequeues.py`
- 2 min: `ImportError: cannot import name 'monitoring_v3' from 'google.cloud' in gcpubsub transport`
- 1 min: `ImportError: The curl client requires the pycurl library (14 SQS test failures)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
