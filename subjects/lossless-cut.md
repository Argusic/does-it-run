# lossless-cut

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mifi/lossless-cut, licensed GPL-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lossless-cut

## Pinned environment

- Project commit: `5af02818fbf0738782e5ac13a4407218b80cc504`
- Test commit: `5af02818fbf0738782e5ac13a4407218b80cc504`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 18.1 to 19.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 18.1 | 4 | 4 | [run](https://argusic.com/run/ebc4d1ec-26a6-45a9-8e8b-de9da16931e3) |
| 2 | pass | 100 | 25 | 18.4 | 6 | 6 | [run](https://argusic.com/run/8a20af6f-739a-4933-9f45-ebce06606c89) |
| 3 | pass | 100 | 19 | 19.7 | 4 | 4 | [run](https://argusic.com/run/857e3e09-68c0-41f8-8347-2cea5e6bf09e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `yarn postinstall (electron-builder install-app-deps) fails on Node 18.19.1 due to @noble/hashes being ESM-only and electron-builder using require()`
- 4 min: `electron's built-in installer fails on Node 18.19.1 due to @electron/get being ESM`
- 2 min: `electron-vite build fails because Vite 7.3.5 uses crypto.hash() which is not available in Node 18`
- 1 min: `2 tests in pathToFileURL.test.ts fail on Node 18 because ^, $, & are not percent-encoded by pathToFileURL`

Attempt 2:

- 3 min: `postinstall script (electron-builder install-app-deps) fails: @noble/hashes is ESM-only`
- 2 min: `pathToFileURL tests fail on Node 18 because ^ is not URL-escaped in Node 18`
- 1 min: `Template literal had double backslash causing double encoding`
- 2 min: `Electron binary not downloaded (ESM error in @electron/get)`
- 1 min: `Electron sandbox helper not configured correctly`
- 2 min: `Build script generateIcon.ts cannot be run with node directly (TS file)`

Attempt 3:

- 1 min: `postinstall script failed: electron-builder install-app-deps requires ESM-only @noble/hashes, incompatible with Node 18`
- 1 min: `yarn build failed: generateIcon.ts can't run directly with Node 18`
- 3 min: `Renderer build OOM (2GB RAM) with sourcemaps enabled`
- 1 min: `Electron binary download fails on Node 18 (ESM @electron/get)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
