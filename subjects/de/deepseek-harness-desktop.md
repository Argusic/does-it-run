# deepseek-harness-desktop

**Verdict: runs.** Argusic Score 98.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ningbainb/deepseek-harness-desktop, licensed BSD-3-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/deepseek-harness-desktop

## Pinned environment

- Project commit: `e6c6756cf14b3064f8953dc37830ac4c06957d51`
- Test commit: `e6c6756cf14b3064f8953dc37830ac4c06957d51`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 22.3 to 49.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96.67 | 12 | 49.7 | 6 | 5 | [run](https://argusic.com/run/0d6fd8ea-db1a-402e-b597-ada16a9b5d38) |
| 2 | pass | 100 | 5 | 22.3 | 5 | 5 | [run](https://argusic.com/run/fdc43c1d-0986-4cc2-87a5-b9b71dede38b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (requires ^22.19.0)`
- 1 min: `pnpm not found`
- 1 min: `7 packages declared packageManager pnpm@11.7.0 conflicting with corepack 11.22.0`
- 1 min: `Playwright chromium-headless-shell not downloaded`
- `ssh-keygen not found (system package, no root)`
- 1 min: `DSH coupling audit stale`

Attempt 2:

- 1 min: `Node.js v18.19.1 is below the project's requirement (^22.19.0)`
- 1 min: `pnpm not found in PATH`
- 1 min: `dsh-ssh prepare failed due to packageManager field declaring pnpm@11.7.0 while corepack runs 11.22.0`
- 2 min: `dsh-desktop integration test fails: Playwright browsers not installed`
- `dsh-ssh engine.test.ts: spawnSync ssh-keygen ENOENT`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
