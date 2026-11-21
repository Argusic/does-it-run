# Financial-API

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Hithink-Tech-Org/Financial-API, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/55efb552-8ba0-4e8a-9cc6-0f3ccaa8a23b

## Pinned environment

- Project commit: `d0856cf522cd5121c44ea3d4e0d2c0aee6974540`
- Test commit: `d0856cf522cd5121c44ea3d4e0d2c0aee6974540`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.9 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 15 | 6.1 | 5 | 5 | [run](https://argusic.com/run/55efb552-8ba0-4e8a-9cc6-0f3ccaa8a23b) |
| 2 | pass with mocks | 92 | 4 | 4.9 | 0 | 0 | [run](https://argusic.com/run/03ead91b-35f9-4827-830f-8a83e8638928) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18.19.1 below CLI requirement ^22.13.0 , import.meta.dirname unsupported`
- 3 min: `Built dist JS files contained import.meta.dirname references`
- 1 min: `assertAuthRuntime refuses Node v18 , blocks auth and remote commands`
- 2 min: `node:sqlite (Node 22+) required by auth-state-lock , not available in v18`
- 1 min: `vitest 4.x (via rolldown) requires Node 21.7+ for styleText , can't run CLI tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
