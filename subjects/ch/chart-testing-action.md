# chart-testing-action

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/helm/chart-testing-action, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/chart-testing-action

## Pinned environment

- Project commit: `f3ef15d8179cc3d72028604dfbf96178583a50a2`
- Test commit: `f3ef15d8179cc3d72028604dfbf96178583a50a2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.1 | 4 | 4 | [run](https://argusic.com/run/843616c7-ce5d-4f73-a63a-b6d2646dfd75) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `cosign binary not found`
- 0.1 min: `uv not found on PATH`
- 0.1 min: `uv not on PATH when ct.sh ran (first attempt found cosign ok but failed at uv venv)`
- 0.2 min: `helm binary not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
