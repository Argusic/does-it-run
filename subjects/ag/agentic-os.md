# agentic-os

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KbWen/agentic-os, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agentic-os

## Pinned environment

- Project commit: `a33cc1145901db0e063f670c33cccca945caf913`
- Test commit: `a33cc1145901db0e063f670c33cccca945caf913`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.3 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 9.3 | 2 | 2 | [run](https://argusic.com/run/2a9cf5df-6210-4ca1-b0bb-2e4d5f6c9032) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `python command not found , only python3 available`
- 1 min: `pytest not installed for system python3`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
