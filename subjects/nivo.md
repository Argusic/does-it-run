# nivo

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/plouc/nivo, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nivo

## Pinned environment

- Project commit: `0dae2c32052a573f9f1d66ec1b453b572119b265`
- Test commit: `0dae2c32052a573f9f1d66ec1b453b572119b265`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 8.4 to 52.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 2.1 | 16.1 | 3 | 0 | [run](https://argusic.com/run/22b4b56d-882a-4104-b627-3c8db4b0eaf2) |
| 1 | pass | 100 | 52 | 52.3 | 1 | 1 | [run](https://argusic.com/run/05fc13e6-5e50-45a0-90db-fe77d25a0f8f) |
| 2 | pass | 100 | 3.5 | 10.8 | 1 | 1 | [run](https://argusic.com/run/71cea70e-ebc0-49f7-9591-692049bea27c) |
| 3 | pass | 100 | 2 | 8.4 | 0 | 0 | [run](https://argusic.com/run/b0d9af98-e52a-424f-8b63-7f14ac129306) |

## What was observed on a clean machine

Attempt 1:

- `Node version mismatch: project requires Node 22.x, container has Node 18.19.1 , cannot upgrade (no root)`
- `Parallel build (pkgs:build) exits with code 123 from xargs spawning sh -c with directories containing parentheses; however all 45 packages successfully built dist/ contents`
- `API runtime fails on Node 18: ERR_REQUIRE_ESM from d3-interpolate being ESM-only in newer versions`

Attempt 1:

- 35 min: `CJS/ESM interop failure: rollup-built CJS bundles require() ES Module d3 packages (d3-interpolate, d3-scale, d3-shape, etc.) on Node 18, causing ERR_REQUIRE_ESM.`

Attempt 2:

- `Node.js version mismatch: project requires 22.x but container has 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
