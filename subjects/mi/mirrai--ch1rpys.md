# Mirrai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ch1rpys/Mirrai, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/01040721-439c-487d-8421-bd83bcfb7671

## Pinned environment

- Project commit: `43fd9daedad4e9c03eb5ed15abd16378eeb5e5ad`
- Test commit: `43fd9daedad4e9c03eb5ed15abd16378eeb5e5ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 15.1 | 5 | 5 | [run](https://argusic.com/run/01040721-439c-487d-8421-bd83bcfb7671) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18 system install insufficient: vitest forks lack globalThis.crypto, breaking jose@6 (JWT lib). 5 tests failed with 'crypto is not defined'`
- 1 min: `pnpm not installed globally (Node 18 system)`
- 5 min: `PostgreSQL not available on system`
- `jsdom test environment fails on Node 18/20: @exodus/bytes ESM require issue in html-encoding-sniffer dependency`
- `Startup warning: no redis-server binary found for rate limiter`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
