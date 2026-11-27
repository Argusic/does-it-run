# VidBee

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nexmoe/VidBee, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vidbee

## Pinned environment

- Project commit: `0d9af1b6a73ac1969441b34addd302b29508cfa7`
- Test commit: `0d9af1b6a73ac1969441b34addd302b29508cfa7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.5 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 4.5 | 4.5 | 4 | 4 | [run](https://argusic.com/run/876a21ff-0b01-45d0-a260-5734ee18b097) |
| 2 | pass | 100 | 7 | 6.1 | 3 | 3 | [run](https://argusic.com/run/42cd5c71-c06d-4dd5-96b7-4dd91feba97b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 installed but project requires v22.22.3 (from .node-version)`
- 0.5 min: `pnpm not found in PATH`
- 0.2 min: `.npmrc had prefix=/home/runner/.npm-global causing EACCES and nvm conflicts`
- `Fastify deprecation warning: disableRequestLogging is deprecated`

Attempt 2:

- 2 min: `pnpm not found in PATH`
- 3 min: `Node.js v18 system but project requires v22`
- 1 min: `WXT postinstall failed with node:util styleText error on Node.js 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
