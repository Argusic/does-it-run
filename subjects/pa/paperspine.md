# PaperSpine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WUBING2023/PaperSpine, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/paperspine

## Pinned environment

- Project commit: `f7e3dabaf499b2aef1eabdd1cd5d64f173d7dcc3`
- Test commit: `f7e3dabaf499b2aef1eabdd1cd5d64f173d7dcc3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 9.5 | 5 | 5 | [run](https://argusic.com/run/9878de95-a414-4072-97f9-b000489e7eeb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 blocks system-level pip install`
- 1 min: `TEST_TEMP_ROOT targets /work/90_临时工作/ which cannot be created without root`
- 0.2 min: `test_workspace context manager is collected as a pytest test function`
- 0.2 min: `.venv directory pollutes scan for private paths in source files`
- 0.5 min: `lxml module missing for word_guard font-repair tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
