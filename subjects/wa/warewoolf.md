# warewoolf

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brsloan/warewoolf, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/warewoolf

## Pinned environment

- Project commit: `5821afcf9c9bb0497a2116a2f1006f451837493b`
- Test commit: `5821afcf9c9bb0497a2116a2f1006f451837493b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 26.8 to 38.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 26.8 | 4 | 4 | [run](https://argusic.com/run/ebc4d9e3-b579-465c-adc6-464b9532a2d4) |
| 2 | pass with mocks | 92 | 28 | 38.1 | 6 | 6 | [run](https://argusic.com/run/539c08f5-de4f-45fb-b121-ce916fa9bb99) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `crypto.randomUUID() not available in node --test mode on Node 18`
- 0.3 min: `jsdom@29 depends on @exodus/bytes (ESM-only), incompatible with require() on Node 18`
- 0.1 min: `MockTimers.enable() takes array form on Node 18, not object form`
- 0.1 min: `hardenDownloadedUpdate() sets 0o400/0o500 permissions causing EACCES on cleanup in updates tests`

Attempt 2:

- 2 min: `Test runner glob pattern not expanded in Node 18`
- 2 min: `MockTimers API expects array, not object, in Node 18`
- 2 min: `jsdom 29.x requires ESM-only dependency @exodus/bytes incompatible with Node 18`
- 3 min: `epub.js uses bare crypto global which is undefined in Node 18 test runner`
- 2 min: `Electron 44 binary download fails in Node 18 (ESM @electron/get)`
- 3 min: `hardenDownloadedUpdate sets chmod 0500 on directory preventing test cleanup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
