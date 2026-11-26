# giselle

**Verdict: runs.** Argusic Score 94 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/giselles-ai/giselle, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/giselle

## Pinned environment

- Project commit: `7dca22434e3dfcd4cf4b32aec20d4d7813a06fb5`
- Test commit: `7dca22434e3dfcd4cf4b32aec20d4d7813a06fb5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 11.4 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 1 | 11.5 | 5 | 4 | [run](https://argusic.com/run/8585cfee-8564-4b33-b862-4d1a2fa734f8) |
| 2 | pass | 100 | 12.4 | 11.4 | 5 | 5 | [run](https://argusic.com/run/ee9c43ed-c660-4b4a-8960-2764a636e8b8) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 installed but project requires >=24`
- 2 min: `pnpm binary not found on PATH`
- 1 min: `npm install -g failed with EACCES`
- 2 min: `Studio build failed due to missing Supabase env vars`
- 3 min: `Production build OOM-killed (exit 137) during page data collection`

Attempt 2:

- 2 min: `pnpm not found in container; had to install via npm -g install`
- 1 min: `Node.js v18 installed but project requires >=24; installed Node.js v22.11.0 from tarball`
- 1 min: `pnpm (via node22's corepack) had a key verification error with standalone pnpm binary`
- 1 min: `turbo subprocesses failed with corepack signature error because PATH inherited corepack shim for pnpm`
- 5 min: `@giselles-ai/nextjs test failed: require() of ESM-only nanoid@5 and title-case@4 from CJS dist of @giselles-ai/utils`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
