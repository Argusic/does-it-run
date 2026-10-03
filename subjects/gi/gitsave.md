# GitSave

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TimWitzdam/GitSave, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/gitsave

## Pinned environment

- Project commit: `da2cc2e14df0c887810171f2dc9a48f56f012838`
- Test commit: `da2cc2e14df0c887810171f2dc9a48f56f012838`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.9 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 9.9 | 2 | 2 | [run](https://argusic.com/run/83a31f51-5621-40fc-8e6e-c5c0e0544471) |
| 2 | pass | 100 | 5 | 14.3 | 1 | 1 | [run](https://argusic.com/run/60e73625-55ab-4aec-8839-7e0e2f0e23fc) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Astro 7 requires Node.js >=22.12.0, system had v18.19.1`
- 0.5 min: `Missing @rolldown/binding-linux-x64-gnu native optional dependency`

Attempt 2:

- 2 min: `Node.js v18.19.1 is too old , Astro v7 and many dependencies require >=22.12.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
