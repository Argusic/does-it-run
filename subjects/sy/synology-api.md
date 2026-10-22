# synology-api

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/N4S4/synology-api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/synology-api

## Pinned environment

- Project commit: `56d514c0c7c4c8c683a65970fa49c797da260317`
- Test commit: `56d514c0c7c4c8c683a65970fa49c797da260317`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.1 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 13.1 | 4 | 4 | [run](https://argusic.com/run/e1230b88-1fbd-4c1c-8e0e-8ba867c70d38) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Externally managed Python environment (Debian) blocks system pip install`
- 5 min: `Missing tests/resources/config-test.json prevents integration tests from running`
- 0.2 min: `tests/test_add_s3_sync_task.py broken import: from setup_tests import parse_config`
- 1 min: `tests/test_core_user.py calls nonexistent methods (get_password_policy, create_user, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
