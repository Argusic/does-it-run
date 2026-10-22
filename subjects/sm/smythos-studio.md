# smythos-studio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SmythOS/smythos-studio, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/smythos-studio

## Pinned environment

- Project commit: `3e1ea87e6718fdfdb24365b2184fbd1daa9f94f8`
- Test commit: `3e1ea87e6718fdfdb24365b2184fbd1daa9f94f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 73.9 to 73.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 75 | 73.9 | 6 | 6 | [run](https://argusic.com/run/f27f3930-dc4f-4876-b269-b8ebbde198f9) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Node.js was 18.19.1 but the repo requires >=20, and pnpm was not installed`
- 5 min: `pnpm 10 ignored postinstall build scripts, so @prisma engines/client were not generated`
- 30 min: `packages/runtime production rollup build OOM-killed in the 2GB container (heap reached ~1.6GB with terser; attempts at 900-1536MB heaps all OOM'd)`
- 12 min: `packages/app frontend bundles (rollup-fe/vanilla) also OOM at ~1.3GB heap in the 2GB container`
- 12 min: `MySQL server is not available and cannot be installed without root; middleware cannot start`
- 4 min: `packages/app backend config prints 'config validation error: "NODE_ENV" is required' and app exits ~15s after start due to missing middleware`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
