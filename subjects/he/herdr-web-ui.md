# herdr-web-ui

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devswha/herdr-web-ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/herdr-web-ui

## Pinned environment

- Project commit: `f35aeae75762245de3b5cc25d0b69832afdd9ad9`
- Test commit: `f35aeae75762245de3b5cc25d0b69832afdd9ad9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 3.1 | 2 | 2 | [run](https://argusic.com/run/74b9c766-dd9e-4270-b60c-c94d72cff7bd) |
| 2 | pass | 100 | 17 | 8.1 | 2 | 2 | [run](https://argusic.com/run/870d8163-d284-4f83-b39d-e9fb9bd9264e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `unzip missing for Bun install script`
- `herdr not installed (0.9.0+ required for plugin-based install)`

Attempt 2:

- 2 min: `Bun not installed; install.sh requires unzip which is not available`
- 1 min: `herdr binary not found for integration tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
