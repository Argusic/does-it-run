# AIPex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AIPexStudio/AIPex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/aipex

## Pinned environment

- Project commit: `4173fa865fed46aa4dd7af19f39a2ecace634116`
- Test commit: `4173fa865fed46aa4dd7af19f39a2ecace634116`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.4 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 4.6 | 3 | 3 | [run](https://argusic.com/run/1cf9692b-00ec-441f-9013-b5c91c400b1a) |
| 2 | pass | 100 | 1.5 | 4.4 | 1 | 1 | [run](https://argusic.com/run/d6486dd4-b595-4d4d-8c34-7b75a590dee7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH`
- 2 min: `Vite 7.3 requires Node ≥20.19; system Node 18.19 rejected by vite build`
- 2 min: `@tailwindcss/oxide-linux-x64-gnu native binding missing (optional dep not fetched by pnpm)`

Attempt 2:

- 3.5 min: `Node 18.19.1 too old , vitest 4.x, vite 7.x, jsdom 29, @vitejs/plugin-react require Node >= 20. Errors: (1) @exodus/bytes ESM/CJS mismatch in jsdom caused ERR_REQUIRE_ESM crash in dom-snapshot, aipex-react, browser-ext tests. (2) @vitejs/pl`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
