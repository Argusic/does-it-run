# smoothui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/educlopez/smoothui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/smoothui

## Pinned environment

- Project commit: `1d61c51eedfac615c26ac1d06d394552d0653ad0`
- Test commit: `1d61c51eedfac615c26ac1d06d394552d0653ad0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 20.2 to 33.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 33.4 | 4 | 4 | [run](https://argusic.com/run/b6d085f0-c35c-4ab9-a355-e74c6717c777) |
| 1 | pass | 100 | 28 | 28.8 | 4 | 4 | [run](https://argusic.com/run/9be0a03f-6303-413c-9274-64d693c677bd) |
| 2 | pass | 100 | 8 | 20.2 | 3 | 3 | [run](https://argusic.com/run/8ac4a287-28da-4e73-82b3-dc77b22f4112) |
| 3 | pass | 100 | 9.2 | 29.1 | 5 | 5 | [run](https://argusic.com/run/02130469-e9bb-4e90-949b-ee4464c9a868) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 is incompatible (project requires >=22.13.0); pnpm not found`
- 2 min: `pnpm-lock.yaml v9 format incompatible with pnpm 8; replaced lockfile`
- 2 min: `nucleo-core-fill-24 preinstall script calls fetch (unavailable in Node 18; fails with exit 1 even without license)`
- 5 min: `Vitest 4 / Vite 8 uses oxc parser instead of esbuild; esbuild.jsx config ignored, causing 'Unexpected JSX expression' parse errors in 123 test files`

Attempt 1:

- 3 min: `Node.js v18.19.1 too old; project requires >=22.13`
- 2 min: `pnpm not installed`
- 2 min: `nucleo-core-fill-24 preinstall script exits 1 without license key ENV var`
- 1 min: `sharp@0.35.3 requires native build from source`

Attempt 2:

- 2 min: `pnpm install failed because nucleo-core-fill-24 preinstall script requires a license key for a commercial icon package (only used in the docs site, not shipped components)`
- 3 min: `Node.js v18 installed but project requires >=22.13.0`
- 5 min: `next build --turbopack failed with SIGSEGV and GitHub API 403 errors from fumadocs-twoslash`

Attempt 3:

- 0.5 min: `Node.js v18.19.1 is too old (requires >=22.13.0)`
- 1.5 min: `pnpm not installed`
- 2 min: `nucleo-core-fill-24 preinstall script requires network license verification to nucleoapp.com API`
- 3 min: `Canvas not installed, causing HTMLCanvasElement getContext() warnings in jsdom tests`
- `.npmrc prefix config causes npm error spam in vitest output`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
