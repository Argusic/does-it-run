# PiBot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/w01fb0ss/PiBot, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pibot

## Pinned environment

- Project commit: `c923b02d8f74108fcb46758bbfc96b39f3cd7de6`
- Test commit: `c923b02d8f74108fcb46758bbfc96b39f3cd7de6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 47 to 47 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 47 | 3 | 3 | [run](https://argusic.com/run/88e6eb63-6066-4799-a1af-6e6f31d499da) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js version mismatch , system has v18.19.1 but project requires v26.11.1`
- 0.5 min: `pnpm 12 not installed , system npm lacks pnpm`
- 3 min: `unzip system binary not available , zip test failed with ENOENT`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
