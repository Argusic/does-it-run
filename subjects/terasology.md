# Terasology

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MovingBlocks/Terasology, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/terasology

## Pinned environment

- Project commit: `f2b8434a2d1d065d8e40173892364c56e7391510`
- Test commit: `f2b8434a2d1d065d8e40173892364c56e7391510`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 23.1 to 40.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 2 | 37.7 | 1 | 1 | [run](https://argusic.com/run/c6b15139-f5a9-45dc-93a1-21784af2707a) |
| 2 | pass | 100 | 22 | 23.1 | 2 | 2 | [run](https://argusic.com/run/29bc8a10-2cf6-446a-bc95-362d7ab2fa54) |
| 3 | pass | 100 | 39 | 40.5 | 2 | 2 | [run](https://argusic.com/run/d4eeea30-7bd5-4406-9e06-56da1595ddb9) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Java JDK 17 not found on system`

Attempt 2:

- 1 min: `No JDK installed in container`
- 10 min: `Headless server failed at runtime: module CoreSampleGameplay not found`

Attempt 3:

- 2 min: `No JDK 17 in container`
- 1 min: `GenericBiomes module.txt uses stale dependency 'Core' (renamed to CoreAssets)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
