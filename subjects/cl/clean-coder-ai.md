# Clean-Coder-AI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Grigorij-Dudnik/Clean-Coder-AI, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/clean-coder-ai

## Pinned environment

- Project commit: `77143dfe50617f8282a2361d1031f561e7043e9e`
- Test commit: `77143dfe50617f8282a2361d1031f561e7043e9e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 3.8 | 1 | 1 | [run](https://argusic.com/run/fdc8d26d-984d-44a0-b965-08c541605b68) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `6 unit tests failed due to argument order mismatch: tests called run_script_in_env(script_name, work_dir) but the function signature is run_script_in_env(work_dir, execute_file_name). Also logs_from_running_script mock assertions had wrong`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
