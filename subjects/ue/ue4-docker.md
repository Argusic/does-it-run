# ue4-docker

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/adamrehn/ue4-docker, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ue4-docker

## Pinned environment

- Project commit: `7f1eccc538b39097f1f196609642cf640d87226e`
- Test commit: `7f1eccc538b39097f1f196609642cf640d87226e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 6.9 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 6.9 | 2 | 2 | [run](https://argusic.com/run/2dafa866-91ca-47ba-a795-affb598472d2) |
| 2 | pass with mocks | 92 | 0.13 | 15.5 | 4 | 4 | [run](https://argusic.com/run/c70155df-32fe-45e8-a320-5829ea9a555f) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `externally-managed-environment prevents system-level pip install`
- 2 min: `Docker daemon not available in container`

Attempt 2:

- 8 min: `Docker daemon not installed in container`
- 0.5 min: `Ubuntu 24.04 externally-managed Python environment blocks system pip install`
- 0.5 min: `info command failed because mock DockerRootDir /var/lib/docker didn't exist`
- 1 min: `setup command failed looking for docker binary in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
