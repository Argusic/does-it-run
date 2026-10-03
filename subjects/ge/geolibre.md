# GeoLibre

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/opengeos/GeoLibre, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/geolibre

## Pinned environment

- Project commit: `3bbeb7b38c8a9781130c5e59e031d3712ffd9749`
- Test commit: `3bbeb7b38c8a9781130c5e59e031d3712ffd9749`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.4 to 22.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 22.4 | 4 | 4 | [run](https://argusic.com/run/9f894cd6-d26e-48b4-91e2-90d73b76d6c9) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 is installed but project requires Node 22+`
- 0.5 min: `Node v22.13.0 lacks registerHooks in node:module (needs >=22.18.0)`
- 0.2 min: `@geolibre/embed dist/ missing , embed-api tests fail with ERR_MODULE_NOT_FOUND`
- 0.1 min: `npm run test:backend uses python but only python3 is available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
