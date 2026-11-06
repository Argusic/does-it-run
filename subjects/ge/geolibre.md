# GeoLibre

**Verdict: runs.** Argusic Score 98.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/opengeos/GeoLibre, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/geolibre

## Pinned environment

- Project commit: `3bbeb7b38c8a9781130c5e59e031d3712ffd9749`
- Test commit: `3bbeb7b38c8a9781130c5e59e031d3712ffd9749`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 22.4 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 22.4 | 4 | 4 | [run](https://argusic.com/run/9f894cd6-d26e-48b4-91e2-90d73b76d6c9) |
| 2 | pass | 97.14 | 30 | 30.3 | 7 | 6 | [run](https://argusic.com/run/a69ed0bf-543e-4434-84d3-f22bb520aa77) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 is installed but project requires Node 22+`
- 0.5 min: `Node v22.13.0 lacks registerHooks in node:module (needs >=22.18.0)`
- 0.2 min: `@geolibre/embed dist/ missing , embed-api tests fail with ERR_MODULE_NOT_FOUND`
- 0.1 min: `npm run test:backend uses python but only python3 is available`

Attempt 2:

- 10 min: `System Node.js 18.19.1 below project's >=22 requirement; Node 18 test runner drops the crypto global causing 366 frontend test failures (crypto is not defined)`
- 2 min: `@geolibre/embed dist/ missing, one test file failed with ERR_MODULE_NOT_FOUND`
- 2 min: `System pip rejected installs (PEP 668 externally-managed-environment)`
- 1 min: `starlette TestClient import failed: requires httpx`
- 2 min: `Two sedona/SQL backend tests failed on missing geopandas`
- 3 min: `python package editable install failed because its build:embed subprocess used Node 18`
- `Rust toolchain not installed so Tauri desktop build was not attempted`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
