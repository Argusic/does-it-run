# meta2d.js

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/le5le-com/meta2d.js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/meta2d-js

## Pinned environment

- Project commit: `a13bf57ae9cac89a6aa562537d9ae2b2bad8b772`
- Test commit: `a13bf57ae9cac89a6aa562537d9ae2b2bad8b772`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 9.5 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 9 | 9.5 | 4 | 4 | [run](https://argusic.com/run/6e36db9c-a4e1-488f-8d03-32fd30820b63) |
| 2 | fail | 80 | 23 | 24.8 | 2 | 2 | [run](https://argusic.com/run/248d02ae-eae5-4604-b486-219647b80cef) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not available; npm install -g pnpm blocked by EACCES on /usr/local/lib`
- 0.5 min: `pnpm install blocked by supply-chain policy on esbuild postinstall script`
- 1 min: `vue-tsc in example app fails with TypeScript 7.0.2 not exporting ./lib/tsc`
- 0.5 min: `vite dev server fails with EMFILE (too many open files) due to low ulimit in container`

Attempt 2:

- 2 min: `pnpm not installed in PATH (needs global install)`
- 1 min: `pnpm install blocked by ERR_PNPM_IGNORED_BUILDS for esbuild`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
