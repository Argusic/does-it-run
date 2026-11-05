# agent-autoloop

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KKKKhazix/agent-autoloop, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agent-autoloop

## Pinned environment

- Project commit: `cecec75be3ca26e6ca1d6833b50152ee9450088d`
- Test commit: `cecec75be3ca26e6ca1d6833b50152ee9450088d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13.4 to 56.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 13.4 | 0 | 0 | [run](https://argusic.com/run/5cf1c796-603a-4aa3-bda4-f0431c0d6223) |
| 2 | pass | 100 | 56 | 56.2 | 5 | 5 | [run](https://argusic.com/run/93a93225-8ffd-414e-ad24-1a41610571f7) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `System Node.js v18.19.1 rejected by install.sh (requires Node >=24); npm install initially ran against wrong engine with EBADENGINE`
- 1 min: `npm test failed with EMFILE 'too many open files' when many test files each spawned file watchers in parallel`
- 18 min: `npm run benchmark fails its '1000 simultaneous long-poll' assertion (only 562-619 active) because server child spawn + sequential fetch on this slow container takes >5s while early polls time out; README documents pass lines as machine-depe`
- 12 min: `simulation.test.ts exhaustive enumeration and full npm test exceed this container's CPU budget (200k-step sim itself completed in ~296s printing valid counts); sim/crash/stream/delivery components pass individually`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
