# supervisor

**Verdict: could not verify.** Not scored (no completed run has a score).

Project: https://github.com/home-assistant/supervisor, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/supervisor

## Pinned environment

- Project commit: `d0d259cf73e9191185b00a2a14c8f8f04b42f9c2`
- Test commit: `d0d259cf73e9191185b00a2a14c8f8f04b42f9c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 87 to 99.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/ca098c1d-8d7f-45f5-a3bf-7ecb201f05b3) |
| 2 | timeout | none | 43 | 99.7 | 6 | 3 | [run](https://argusic.com/run/e1ab02ff-9af1-49b9-aa46-4a74d8a3e87d) |

## What was observed on a clean machine

Attempt 2:

- 22 min: `Python 3.12 in container, project requires >=3.14`
- 2 min: `Pip install blocked by externally-managed-environment`
- `Python 3.14 syntax (except TypeA, TypeB:) not parseable on 3.12`
- `3 test failures in hardware/test_disk.py (pre-existing, testing directory sizes that are 0 in container)`
- `1 test failure in mounts/test_manager.py (pre-existing, cannot determine image from metadata)`
- `Some test modules (test_app.py, test_manager.py, API tests) hang due to Docker daemon not being available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
