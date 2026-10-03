# tilemill

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tilemill-project/tilemill, licensed BSD-3-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/tilemill

## Pinned environment

- Project commit: `d2c8348aa8d01ffb4607a04bb4b9c9d948df2560`
- Test commit: `d2c8348aa8d01ffb4607a04bb4b9c9d948df2560`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 39.5 to 39.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 39.5 | 5 | 5 | [run](https://argusic.com/run/3704a45b-2ab4-41a8-9cb9-35477688816e) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `npm install failed on native modules (mapnik, gdal, sqlite3, zipfile) - node-pre-gyp cannot download pre-built binaries (HTTP 403 from S3) and source compilation fails against system Mapnik 3.1 (node-mapnik 3.7.2 expects Mapnik 3.0.20 heade`
- 5 min: `node 18.19.1 not supported - TileMill requires node 8.x`
- `PostgreSQL/PostGIS not available - 3 datasource tests fail`
- `Tile rendering tests fail - mock mapnik cannot produce real PNG tiles`
- `Export anti-meridian test fails - S3 download URL returns 403`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
