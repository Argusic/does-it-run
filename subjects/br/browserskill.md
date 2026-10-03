# BrowserSkill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Tencent/BrowserSkill, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/browserskill

## Pinned environment

- Project commit: `f62e283cbb848118096491d1926d8714ebf05b8f`
- Test commit: `f62e283cbb848118096491d1926d8714ebf05b8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.1 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 17.1 | 3 | 3 | [run](https://argusic.com/run/f51d542e-eb9f-4be1-b73a-3b4a97c81ec0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18 (v18.19.1) lacks 'styleText' in 'node:util', which rolldown/vitest dependency requires`
- 1 min: `rolldown native bindings built for Node 18 were incompatible after switching to Node 22`
- 1 min: `vitest could not find '.wxt/tsconfig.json' needed by vite:oxc plugin`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
