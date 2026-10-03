# mcphub

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/samanhappy/mcphub, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcphub

## Pinned environment

- Project commit: `9cf6c1b8b78f86af2c9cab592e3589a9ce5b4cbb`
- Test commit: `9cf6c1b8b78f86af2c9cab592e3589a9ce5b4cbb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 76.4 to 76.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 76.4 | 3 | 3 | [run](https://argusic.com/run/0388a7b3-31d2-4e8d-8ca4-014ba494c35b) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `pnpm not found in PATH`
- 3 min: `serverController-toggleTool-live-config.test.ts and openApiController.yaml.test.ts fail due to Node 18 + Jest + pkce-challenge dynamic import('node:crypto') incompatibility`
- `Frontend vite build hangs for >30s on transforming 1902 modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
