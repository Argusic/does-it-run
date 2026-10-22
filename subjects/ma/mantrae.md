# mantrae

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MizuchiLabs/mantrae, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mantrae

## Pinned environment

- Project commit: `10e1ee319e7e2ac5fbab1db8bf14ba275c72c024`
- Test commit: `10e1ee319e7e2ac5fbab1db8bf14ba275c72c024`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 10.8 | 3 | 3 | [run](https://argusic.com/run/784c80f8-02b7-496f-bb78-d879351284b3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not pre-installed`
- 1 min: `Node.js v18 too old for rolldown (needs node:util.styleText from Node 22+)`
- 0.5 min: `Initial pnpm install under Node 18 downloaded wrong native bindings for rolldown`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
