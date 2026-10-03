# qor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qor/qor, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/qor

## Pinned environment

- Project commit: `79e51bd0739a481b01546642db390f070dae57f3`
- Test commit: `79e51bd0739a481b01546642db390f070dae57f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.6 to 39.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 39 | 39.6 | 3 | 3 | [run](https://argusic.com/run/5186554d-feb7-4f70-a2fa-4e88473c9a1c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`
- 23 min: `No database server available for tests`
- 1 min: `Gulp frontend build fails because admin views are in a separate sibling repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
