# mycart

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shurco/mycart, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mycart

## Pinned environment

- Project commit: `c3987312b72f222f4f0ad5507164bad67fe067be`
- Test commit: `c3987312b72f222f4f0ad5507164bad67fe067be`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.6 | 4 | 4 | [run](https://argusic.com/run/8798bcb9-28e2-4ca2-b2cf-e00ea5468294) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go binary not installed in environment`
- 1 min: `Package github.com/shurco/mycart/docs/swagger could not be resolved , Swagger docs not generated`
- 3 min: `Frontend build directories (admin/build, site/build) missing , Go :go:embed directive failed`
- 2 min: `npm ci failed due to Node.js v18 engine requirements and dependency lock conflicts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
