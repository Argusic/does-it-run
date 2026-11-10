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
- Valid runs: 2; wall time 39.5 to 52.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 39.5 | 5 | 5 | [run](https://argusic.com/run/3704a45b-2ab4-41a8-9cb9-35477688816e) |
| 2 | pass with mocks | 92 | 10 | 52.8 | 4 | 4 | [run](https://argusic.com/run/b3b6b2d4-c66c-4525-b4c6-f5dd0fcdbbc3) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `npm install failed on native modules (mapnik, gdal, sqlite3, zipfile) - node-pre-gyp cannot download pre-built binaries (HTTP 403 from S3) and source compilation fails against system Mapnik 3.1 (node-mapnik 3.7.2 expects Mapnik 3.0.20 heade`
- 5 min: `node 18.19.1 not supported - TileMill requires node 8.x`
- `PostgreSQL/PostGIS not available - 3 datasource tests fail`
- `Tile rendering tests fail - mock mapnik cannot produce real PNG tiles`
- `Export anti-meridian test fails - S3 download URL returns 403`

Attempt 2:

- 20 min: `Native C++ modules (mapnik, sqlite3, gdal, zipfile) require pre-built binaries from mapbox-node-binary S3, which returned 403 for node v18. Source compilation also fails: mapnik needs system libmapnik (mapnik-config missing), gdal needs lib`
- `npm ls command format changed in modern npm (v9+), causing duplicate_module.test.js to fail for optimist module.`
- `PostgreSQL/PostGIS not available in container. Datasource tests (datasource.test.js) require psql, createdb, and template_postgis database.`
- `Tile/grid render and anti-meridian export tests time out because the mapnik mock returns empty image buffers instead of rendering real tiles. Mapnik.Backend waits for render completion which never happens when images are empty zero-byte buf`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
