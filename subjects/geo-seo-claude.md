# geo-seo-claude

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zubair-trabzada/geo-seo-claude, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/geo-seo-claude

## Pinned environment

- Project commit: `9b911b00aea2635d5cc35847b96bb6f84a48ab8e`
- Test commit: `9b911b00aea2635d5cc35847b96bb6f84a48ab8e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 3.2 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 9.3 | 0 | 0 | [run](https://argusic.com/run/66b6b1b3-5cd1-49c4-81d3-b25e88304398) |
| 2 | pass with mocks | 92 | 0.1 | 3.2 | 0 | 0 | [run](https://argusic.com/run/ae50dd57-ce71-477f-b1c0-31006c519953) |
| 3 | pass | 100 | 2 | 3.3 | 2 | 2 | [run](https://argusic.com/run/57d9b4da-63ab-4f42-b5be-25c291ec5681) |

## What was observed on a clean machine

Attempt 3:

- 0.5 min: `externally-managed-environment blocked system pip install`
- 0.1 min: `pytest not installed (not in requirements.txt)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
