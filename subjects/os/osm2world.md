# OSM2World

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tordanik/OSM2World, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/osm2world

## Pinned environment

- Project commit: `8ec26a9ea426444a4f7882cf0cfcab432c876ae5`
- Test commit: `8ec26a9ea426444a4f7882cf0cfcab432c876ae5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.5 to 19.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 19.6 | 2 | 2 | [run](https://argusic.com/run/08797069-8e7e-4f2a-8e76-b4d5646e2c7f) |
| 2 | pass | 100 | 14.9 | 14.5 | 2 | 2 | [run](https://argusic.com/run/dbfc1a73-d8af-4b01-bbe9-d3d274fc3e5b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Java or Maven installed in container`
- 5 min: `jogamp.org (source for JOGL 2.4.0) unreachable - connection timed out`

Attempt 2:

- 2 min: `JOGL dependencies from jogamp.org unreachable (connection refused)`
- 1 min: `FrontendPbfOutputTest failed: 'No platform-specific image implementation provided'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
