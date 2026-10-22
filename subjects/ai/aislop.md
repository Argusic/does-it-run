# aislop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scanaislop/aislop, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/aislop

## Pinned environment

- Project commit: `3f5d5bba3794ba1bab19383191dd2509d6b4dded`
- Test commit: `3f5d5bba3794ba1bab19383191dd2509d6b4dded`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.7 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 12.7 | 5 | 5 | [run](https://argusic.com/run/c359d330-9e66-4830-921f-36fd2606c839) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (requires >=20)`
- 1 min: `pnpm not installed`
- 3 min: `Rolldown native binding @rolldown/binding-linux-x64-gnu missing (optional dep)`
- 2 min: `unrun peer dependency of tsdown not installed`
- 1 min: `Node 20 styleText API incompatibility with rolldown`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
