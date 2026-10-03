# anything-analyzer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mouseww/anything-analyzer, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/anything-analyzer

## Pinned environment

- Project commit: `1da6b5c9acc024e987d41e4b9c88676ffea0da0c`
- Test commit: `1da6b5c9acc024e987d41e4b9c88676ffea0da0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 9.1 | 4 | 4 | [run](https://argusic.com/run/e4c4eb03-8d41-4728-bc8d-361630bf7a89) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not available , installed via npm`
- 1 min: `vitest 3.x incompatible with Node 18.19.1 (ESM/CJS error)`
- 1 min: `Electron binary absent , build scripts blocked by pnpm`
- 1 min: `mcp-server-listen.test.ts failed , electron import not available in vitest node environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
