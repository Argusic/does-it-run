# AnyModelBot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modelflare-ai/AnyModelBot, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/anymodelbot

## Pinned environment

- Project commit: `c4b0e5f17f601429f7f58a0e0fc1e47dd93fa099`
- Test commit: `c4b0e5f17f601429f7f58a0e0fc1e47dd93fa099`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13.2 to 18.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13.2 | 2 | 2 | [run](https://argusic.com/run/bda1896a-5865-46b2-8ec7-ef3622b8f0c5) |
| 2 | pass | 100 | 8 | 18.5 | 2 | 2 | [run](https://argusic.com/run/aed74ca2-ee4d-46ea-9448-3f8433d50ce1) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `git submodule vendor/magpie commit hash e4ca47b0 does not exist on remote anymore; clone failed with 'Unable to find current revision'`
- 3 min: `Node.js 18.19.1 is installed but project requires >=22.13; Go is not installed but project requires 1.26.8+`

Attempt 2:

- 1 min: `System Node.js is v18.19.1, but the project requires >=22.13 , had to download and use Node v22.13.0 binary from nodejs.org`
- 1 min: `System Go is not installed; the project requires Go >=1.26.8 to compile the magpie gateway`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
