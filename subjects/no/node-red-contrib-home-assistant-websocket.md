# node-red-contrib-home-assistant-websocket

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zachowj/node-red-contrib-home-assistant-websocket, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/node-red-contrib-home-assistant-websocket

## Pinned environment

- Project commit: `978cdbcd3c7c231c7417e624e7fe066df8de2eb2`
- Test commit: `978cdbcd3c7c231c7417e624e7fe066df8de2eb2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 2.1 | 2 | 2 | [run](https://argusic.com/run/af362770-87d2-4aae-bb73-637e9a3fd6c0) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `system Node.js v18.19.1 does not meet minimum requirement v20+ (engines.node >=20)`
- 0.5 min: `pnpm not on PATH with the correct Node version; corepack unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
