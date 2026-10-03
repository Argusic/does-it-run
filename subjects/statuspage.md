# statuspage

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/statsig-io/statuspage, licensed ISC, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/statuspage

## Pinned environment

- Project commit: `4edbee1a8c91bf1fd2c6091154d0743d48190784`
- Test commit: `4edbee1a8c91bf1fd2c6091154d0743d48190784`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.9 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 12.2 | 1 | 1 | [run](https://argusic.com/run/3c2b9a87-4197-48bf-bd9a-860fde9fb1bf) |
| 2 | pass | 100 | 0 | 2.9 | 0 | 0 | [run](https://argusic.com/run/e7fcf3f2-c658-4c85-acc1-73b8f494403a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `worldclockapi.com endpoint is unreachable (connection timeout), causing health-check.sh to hang indefinitely`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
