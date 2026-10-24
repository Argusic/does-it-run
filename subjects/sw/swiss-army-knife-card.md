# swiss-army-knife-card

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AmoebeLabs/swiss-army-knife-card, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/swiss-army-knife-card

## Pinned environment

- Project commit: `57edfa806a91661386568dd67915ef622f2a8f70`
- Test commit: `57edfa806a91661386568dd67915ef622f2a8f70`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 4.9 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 5.4 | 1 | 1 | [run](https://argusic.com/run/172bc592-476b-402d-83a7-a9c39ce0edc8) |
| 2 | fail | 80 | 8 | 4.9 | 1 | 1 | [run](https://argusic.com/run/fa6279e0-8640-4657-ace9-61a27f6843cf) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Rollup build failed with 'crypto is not defined' error from serialize-javascript@7.0.5 (dependency of @rollup/plugin-terser) because bare 'crypto' browser API doesn't exist in Node 18.19 Worker thread context`

Attempt 2:

- 3 min: `Node 18 worker threads lack globalThis.crypto; serialize-javascript crashed with 'crypto is not defined' when @rollup/plugin-terser spawned a worker`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
