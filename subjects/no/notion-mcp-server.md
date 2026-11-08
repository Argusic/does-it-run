# notion-mcp-server

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/makenotion/notion-mcp-server, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/notion-mcp-server

## Pinned environment

- Project commit: `730ae781ba28beeaf0865025a3f2ed4c25ea2387`
- Test commit: `730ae781ba28beeaf0865025a3f2ed4c25ea2387`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.7 to 13.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.7 | 1 | 1 | [run](https://argusic.com/run/288e6e92-bd7b-4c48-995f-69bb2626f0f6) |
| 2 | pass with mocks | 92 | 13.4 | 13.2 | 2 | 2 | [run](https://argusic.com/run/583ef1b7-e706-4b5e-99a5-2c2609a5b46b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `vitest 4.x requires Node >=20, but container has Node 18.19.1 , 'npm test' fails with SyntaxError: The requested module 'node:util' does not provide an export named 'styleText'`

Attempt 2:

- 0.3 min: `vitest v4 requires Node.js >=20, but Node 18 is installed`
- 0.8 min: `crypto.randomUUID is not defined as a bare global in Node 18 ESM bundled code, causing Parse error on initialization`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
