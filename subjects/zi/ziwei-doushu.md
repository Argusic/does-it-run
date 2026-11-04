# ziwei-doushu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Renhuai123/ziwei-doushu, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ziwei-doushu

## Pinned environment

- Project commit: `9d98b3ae7fce298f751cb43c47783d6e84a7735d`
- Test commit: `9d98b3ae7fce298f751cb43c47783d6e84a7735d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.47 | 3 | 0 | 0 | [run](https://argusic.com/run/9b62a87c-f846-4169-a071-c146fe9a46f3) |
| 2 | pass | 100 | 5 | 5.4 | 3 | 3 | [run](https://argusic.com/run/1227b99d-0194-423e-944e-07e6ff791015) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Engine check script failed with MODULE_NOT_FOUND for './lib/ziwei/algorithm' when run from /tmp (relative import resolved against script dir)`
- 1 min: `Production server appeared ready but was killed when the launching shell exited, so curls returned 000 connection refused`
- 3 min: `/knowledge/[star]/[topic] detail pages return 404 (NoFallbackError in server log)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
