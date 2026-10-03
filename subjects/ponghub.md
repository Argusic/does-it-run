# PongHub

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DevXDojo/PongHub, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/ponghub

## Pinned environment

- Project commit: `55efed86a221e09c84eff1987d6e2e2bb997c092`
- Test commit: `55efed86a221e09c84eff1987d6e2e2bb997c092`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.4 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.1 | 9.3 | 0 | 0 | [run](https://argusic.com/run/dd9b06f2-b507-481a-8c59-59acdde9a5e6) |
| 2 | pass | 100 | 3.5 | 4.4 | 1 | 1 | [run](https://argusic.com/run/14ec9bed-04de-4976-bb6f-f311f3a12579) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Go 1.24.5 not pre-installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
