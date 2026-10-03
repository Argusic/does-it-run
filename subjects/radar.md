# radar

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/skyhook-io/radar, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/radar

## Pinned environment

- Project commit: `74ddfa9b88a0eade11457b95c7c4ce9db17780d4`
- Test commit: `74ddfa9b88a0eade11457b95c7c4ce9db17780d4`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 21.5 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/f8f8a726-ef11-4c5d-b136-1cd6f8098b8e) |
| 1 | pass with mocks | 92 | 21 | 21.5 | 3 | 3 | [run](https://argusic.com/run/26a7cfe5-d114-40b2-b485-98c3410f817d) |
| 2 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/bbd9802a-4475-459c-880c-99330e790338) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed (required Go 1.26+)`
- 2 min: `Node.js v18.19.1 is too old (project requires >=20)`
- 1 min: `Timeline test TestSQLiteStore_StartCleanupLoop_PrunesByMaxSizeWithoutRetention had a race/deadline of 2s that was too short`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
