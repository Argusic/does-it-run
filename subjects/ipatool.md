# ipatool

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/majd/ipatool, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/ipatool

## Pinned environment

- Project commit: `8f9748fa51c36cb5f746749170fabcf5e80298d7`
- Test commit: `8f9748fa51c36cb5f746749170fabcf5e80298d7`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 2 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.46 | 8.3 | 2 | 2 | [run](https://argusic.com/run/8885a66d-330e-4987-a617-c84d42110c6a) |
| 2 | pass with mocks | 92 | 1 | 2 | 0 | 0 | [run](https://argusic.com/run/f8bb4d4f-4c58-4c3d-bf25-6ad5741363cf) |
| 3 | pass | 100 | 2 | 6 | 1 | 1 | [run](https://argusic.com/run/962d8454-80a4-4f59-8601-932350542db4) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Go compiler not found in container`
- 0.12 min: `1password/onepassword-sdk-go fails to compile without CGO: references undefined ERROR identifier`

Attempt 3:

- 1 min: `go binary not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
