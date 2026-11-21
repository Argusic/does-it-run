# OpenCompany

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zeenie-ai/OpenCompany, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/opencompany

## Pinned environment

- Project commit: `261cf9391f455418ff5a48c5c193796737e6cd02`
- Test commit: `261cf9391f455418ff5a48c5c193796737e6cd02`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.6 | 9.3 | 3 | 3 | [run](https://argusic.com/run/48cac133-3582-49da-873a-bebf4b7e8008) |
| 2 | pass | 100 | 5.2 | 6 | 4 | 4 | [run](https://argusic.com/run/968445ee-dce3-4437-80be-f815d46520c4) |

## What was observed on a clean machine

Attempt 1:

- 0.02 min: `bun not pre-installed in container`
- 0.01 min: `uv not pre-installed in container`
- 0.01 min: `bun official installer requires unzip; not available`

Attempt 2:

- 1 min: `bun not found in container , needed to install/build`
- 1 min: `python command not found , only python3 available`
- 1 min: `uv not found; pip install uv failed with externally-managed-environment`
- 1 min: `PEP 668 externally-managed-environment blocked pip install -e . for CLI dependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
