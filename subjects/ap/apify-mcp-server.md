# apify-mcp-server

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apify/apify-mcp-server, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/apify-mcp-server

## Pinned environment

- Project commit: `f9b4c7764587483780d8788097d2ab97c8d263a1`
- Test commit: `f9b4c7764587483780d8788097d2ab97c8d263a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 3.1 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 4.5 | 0 | 0 | [run](https://argusic.com/run/418ac168-2231-4bd7-a77a-c174d59dddd0) |
| 2 | pass | 100 | 5 | 6.8 | 2 | 2 | [run](https://argusic.com/run/a8683a70-ca20-44d9-b5a4-807eefecdd35) |
| 3 | fail | 20 | n/a | 3.1 | 0 | 0 | [run](https://argusic.com/run/60ee819d-da20-40ea-9ac2-9045812f6bd3) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Node.js v18.19.1 below project minimum (>=22) and pnpm not found`
- 2 min: `oxlint config parsing failed with Node.js v22.14.0 (needs >=22.18.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
