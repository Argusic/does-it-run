# Monogatari

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Monogatari/Monogatari, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/monogatari

## Pinned environment

- Project commit: `86659baf065178071f0956092f754e1d76be0072`
- Test commit: `86659baf065178071f0956092f754e1d76be0072`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 12.3 to 27.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 27.5 | 4 | 4 | [run](https://argusic.com/run/8018f964-63c2-4aa6-bfad-2a83aa9fa55f) |
| 2 | fail | 20 | n/a | 12.3 | 0 | 0 | [run](https://argusic.com/run/59fda487-7688-4610-b930-baae03cb91d7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not found in container`
- 3 min: `Cypress bundled tsx incompatible with Node v18.19.1 (--loader deprecated)`
- 2 min: `cypress.config.js uses require() but package.json is type:module`
- 1 min: `Electron renderer crash on show_character.spec.js under heavy load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
