# lasso

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sammyjo20/lasso, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/lasso

## Pinned environment

- Project commit: `c39cdd7967d5d367fd4eb25f1d4d91597a9a67f3`
- Test commit: `c39cdd7967d5d367fd4eb25f1d4d91597a9a67f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.9 to 11.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 11.9 | 1 | 1 | [run](https://argusic.com/run/f62642a2-13e6-4b05-ba65-58051aa0acd2) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `webpackbar@5.0.2 ProgressPlugin options rejected by webpack v5.112.2 strict schema validation , 'name', 'color', 'reporters', 'reporter' are not valid ProgressPlugin options`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
