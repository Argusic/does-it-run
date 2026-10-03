# tabby

**Verdict: could not verify.** Argusic Score 70 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Eugeny/tabby, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tabby

## Pinned environment

- Project commit: `14e2d60b9b6dee84a53c37f05eefeb803787de04`
- Test commit: `14e2d60b9b6dee84a53c37f05eefeb803787de04`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 3; wall time 13.5 to 17.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 12.2 | 13.5 | 4 | 4 | [run](https://argusic.com/run/774123b4-5aae-4009-aa90-9edeecc55d11) |
| 2 | fail | 80 | 17 | 16.8 | 3 | 3 | [run](https://argusic.com/run/39889781-4cd2-4b0e-a17d-4b7ddce1a9bf) |
| 3 | fail | 80 | 12 | 17.3 | 8 | 8 | [run](https://argusic.com/run/703a7227-35dc-4807-be7f-ad68ae457928) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `ESM/CJS incompatibility: npmlog/gauge/wide-align required string-width (ESM v5) via require() on Node 18`
- 1 min: `node-abi@4.9.0 requires Node >=22.12.0 but Node 18.19.1 is installed`
- 0.5 min: `yarn not found in PATH (installed in npx cache)`
- 3 min: `System libraries missing for Electron (glib, nss, gtk, X11, etc. - ~25 libs missing from isolated container)`

Attempt 2:

- 1 min: `Yarn not installed`
- 2 min: `Node.js 18 incompatible with node-abi v4 (requires >=22)`
- 5 min: `Missing make/gcc for native module rebuild via @electron/rebuild`

Attempt 3:

- 1 min: `yarn not on PATH`
- 1 min: `node-abi@4.24.0 requires Node >=22, have Node 18`
- 1 min: `git describe --tags fails: no tags`
- 3 min: `string-width@5.1.2 ESM-only breaks CJS npmlog/wide-align via type:module in package.json`
- 2 min: `strip-ansi@7.1.2 ESM-only breaks CJS string-width-cjs`
- 1 min: `yarn not found in subdirectory install-deps.mjs script (PATH issue)`
- 1 min: `marked@18 engine incompatibility in tabby-settings`
- 2 min: `keytar native build fails: libsecret-1-dev not installed, no root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
