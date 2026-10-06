# browserless

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microlinkhq/browserless, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/browserless

## Pinned environment

- Project commit: `56b046acc55c9315d068580929b9e00a033d5f63`
- Test commit: `56b046acc55c9315d068580929b9e00a033d5f63`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.5 to 32.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 2 | 32.5 | 6 | 4 | [run](https://argusic.com/run/d4f2f8c8-43b1-4613-babc-7df82496c1d3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 too old (required >= 24)`
- 1 min: `pnpm not installed`
- 1 min: `puppeteer v25 is ESM-only; require() fails without --experimental-require-module`
- 1 min: `sharp optional dep @img/sharp-linux-x64 not resolved by pnpm`
- `3 screenshot tests fail pixel-diff comparison (environment variation)`
- `1 idempotency test expects eager browser creation; browserless factory is lazy`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
