# esp32-ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/slvDev/esp32-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/esp32-ai

## Pinned environment

- Project commit: `52ebcbbd905270592c1d415efd1128d04d0fa365`
- Test commit: `52ebcbbd905270592c1d415efd1128d04d0fa365`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.6 to 22.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 2.6 | 0 | 0 | [run](https://argusic.com/run/4eeade11-4113-48ae-8919-43595ace4066) |
| 2 | pass | 100 | 12 | 22.2 | 1 | 1 | [run](https://argusic.com/run/251329e3-0f2f-4718-a81f-37944bb2c6ec) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `ModuleNotFoundError: No module named 'model' when running tests without PYTHONPATH set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
