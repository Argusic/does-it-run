# lobe-tts

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lobehub/lobe-tts, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lobe-tts

## Pinned environment

- Project commit: `d61d820d04ca6ea3d9bdea190f9666736ac87e98`
- Test commit: `d61d820d04ca6ea3d9bdea190f9666736ac87e98`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 10 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 17.5 | 5 | 5 | [run](https://argusic.com/run/306b930f-a48c-4999-8ef3-adb5cc1e5a4b) |
| 2 | pass with mocks | 92 | 9.2 | 10 | 3 | 3 | [run](https://argusic.com/run/425acaa9-3a21-45c9-b765-14ea2e82fb1e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install ERESOLVE: dumi-theme-lobehub requires @lobehub/ui ^4.3.3 but project pins ^5.0.0`
- 2 min: `prepare script (husky && dumi setup) crashes on Node 18 with ERR_REQUIRE_ESM requiring ESM chalk`
- 1 min: `npm run build on Node 18: tsdown/rolldown fails, node:util has no styleText export and rolldown native binding is missing`
- 1 min: `README Node.js example and testing need the ws polyfill, which is not a package dependency`
- 6 min: `E2E WebSocket mock did not respond because I matched header 'Path: ssml' with a space but the library sends 'Path:ssml'`

Attempt 2:

- 1 min: `npm install without --legacy-peer-deps fails with 'Cannot read properties of null (reading edgesOut)'`
- 3 min: `tsdown build fails because Node v18 lacks node:util styleText export (requires Node 20+)`
- 1 min: `vitest jsdom environment breaks on Node 18 because jsdom v27 is ESM-only`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
