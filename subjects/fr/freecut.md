# freecut

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/walterlow/freecut, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/freecut

## Pinned environment

- Project commit: `4d62e8082c5eb387a96275bcbd323d28f6e41a62`
- Test commit: `4d62e8082c5eb387a96275bcbd323d28f6e41a62`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 40 to 43.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 41 | 42.4 | 2 | 2 | [run](https://argusic.com/run/fee28446-2459-4c5c-a756-0ffa359198e9) |
| 1 | pass | 100 | 17 | 40 | 3 | 3 | [run](https://argusic.com/run/dff0d555-ae67-4b80-9160-89debf3deda4) |
| 2 | timeout | none | 43 | 43.8 | 5 | 5 | [run](https://argusic.com/run/ba64f93f-270c-4b5f-a754-c31c63ac36a0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (needs >=20.19); vite-plus imports node:util.styleText which is unavailable`
- 1 min: `Headless Chrome tests (channel: 'chrome') require full Google Chrome binary, cannot install without root`

Attempt 1:

- 1 min: `Node.js v18.19.1 is too old for TypeScript 7 and vite-plus (needs >=20)`
- 1 min: `npm install --ignore-scripts skipped optional native bindings for vite-plus`
- 3 min: `Playwright headless scripts use channel:'chrome' which requires system Chrome binary not available in container`

Attempt 2:

- 2 min: `Node.js v18 too old , vite-plus/vite 8 require Node >=20.19`
- 1 min: `rolldown native binding linux-x64-gnu not installed`
- 5 min: `navigator undefined in decoder-prewarm.ts and projects.ts in Node test envs`
- 8 min: `headless tests require channel:chrome (system Chrome not installed)`
- `313 fork worker startup errors from html-encoding-sniffer require() of ESM @exodus/bytes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
