# terragrunt

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gruntwork-io/terragrunt, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/terragrunt

## Pinned environment

- Project commit: `65dc2de2690cb23a915b8e63350d05402f8e490e`
- Test commit: `65dc2de2690cb23a915b8e63350d05402f8e490e`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 12.7 to 26.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.7 | 0 | 0 | [run](https://argusic.com/run/c4b71123-7efd-48a4-89e2-239ab382dd84) |
| 2 | pass with mocks | 92 | 10 | 17.2 | 0 | 0 | [run](https://argusic.com/run/ebcc3683-8345-4c4d-8035-706b374f614a) |
| 3 | pass with mocks | 92 | 43 | 26.9 | 2 | 2 | [run](https://argusic.com/run/13ba53ca-72cd-49a1-80e7-c7698f4f2808) |

## What was observed on a clean machine

Attempt 3:

- 3 min: `Go 1.27 not installed in container`
- 1 min: `/tmp/terragrunt binary file conflicted with provider cache service default path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
