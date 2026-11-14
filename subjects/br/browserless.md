# browserless

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microlinkhq/browserless, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/browserless

## Pinned environment

- Project commit: `56b046acc55c9315d068580929b9e00a033d5f63`
- Test commit: `56b046acc55c9315d068580929b9e00a033d5f63`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 25.5 to 32.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 2 | 32.5 | 6 | 4 | [run](https://argusic.com/run/d4f2f8c8-43b1-4613-babc-7df82496c1d3) |
| 2 | pass | 100 | 0.5 | 25.5 | 3 | 3 | [run](https://argusic.com/run/0b40cefb-c550-4244-bb07-a22d0e97d85d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 too old (required >= 24)`
- 1 min: `pnpm not installed`
- 1 min: `puppeteer v25 is ESM-only; require() fails without --experimental-require-module`
- 1 min: `sharp optional dep @img/sharp-linux-x64 not resolved by pnpm`
- `3 screenshot tests fail pixel-diff comparison (environment variation)`
- `1 idempotency test expects eager browser creation; browserless factory is lazy`

Attempt 2:

- 1 min: `Node.js version mismatch: container has v18.19.1, project requires >= 24`
- 7 min: `sharp native optional dependency (@img/sharp-linux-x64) not installed - pnpm skipped it`
- `Screenshot pixel-diff threshold: project expects 0 diff without CI env, but rendered screenshots vary slightly across Chrome versions (1132, 2015, 1132 pixels diff)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
