# pad

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PerpetualSoftware/pad, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/pad

## Pinned environment

- Project commit: `512343853906c858466e3e5105212de9970445df`
- Test commit: `512343853906c858466e3e5105212de9970445df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 40.5 to 40.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 40.5 | 4 | 4 | [run](https://argusic.com/run/ca0c2436-2997-4076-a1ad-2f3a178c29f3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in environment`
- 3 min: `Node.js v18 too old for project dependencies (requires ^22.22.2 || ^24.15.0 || >=26.0.0)`
- 1 min: `make build-go failed: embed.go requires web/build directory which needs web UI build first`
- 5 min: `14 tests in internal/buildtools fail due to missing ss/lsof commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
