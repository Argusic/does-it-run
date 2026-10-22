# node-red-contrib-uibuilder

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TotallyInformation/node-red-contrib-uibuilder, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/node-red-contrib-uibuilder

## Pinned environment

- Project commit: `f9066f0f6a06f042ec9e41e89285a3603e86cf0c`
- Test commit: `f9066f0f6a06f042ec9e41e89285a3603e86cf0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.5 to 35.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34.3 | 35.5 | 5 | 5 | [run](https://argusic.com/run/2dcc1b0d-c85e-483a-925b-9723c0399264) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `npm install and build succeeded but installed package could not build: ERR_MODULE_NOT_FOUND esbuild in bin/build.mjs (esbuild is devDependency, excluded from published tarball)`
- 18 min: `Node 18.19.1 + jsdom 29/undici 7/parse5 8: ERR_REQUIRE_ESM and missing File/ArrayBuffer.resizable break require('jsdom') (uib-html node fails to load)`
- 6 min: `uibuilder 'get page meta' control handler crashes on deployed node: path.join(undefined) because sourceFolder was left undefined`
- 4 min: `Socket.IO polling transport fails against this server (xhr poll error) on Node 18`
- 7 min: `wrangler 4 requires Node 22 and real Cloudflare creds for remote D1; local D1 ran but worker returned 500 (no schema) then 401 (no STATS_TOKEN secret)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
