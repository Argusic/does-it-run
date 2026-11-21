# dsh-browser

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/omdsh-dev/dsh-browser, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-browser

## Pinned environment

- Project commit: `36fd3ad2d22b814d462b158541c843e6df0bb1cd`
- Test commit: `36fd3ad2d22b814d462b158541c843e6df0bb1cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.7 to 27.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18.5 | 27.8 | 4 | 4 | [run](https://argusic.com/run/600f9549-b701-4b32-931b-8bb27329f582) |
| 2 | pass | 100 | 3.9 | 7.7 | 4 | 4 | [run](https://argusic.com/run/27a6e2c5-d931-43f7-9848-22621bef6b55) |

## What was observed on a clean machine

Attempt 1:

- 0.8 min: `Node.js v18 too old (needs ^22.19)`
- 0.4 min: `pnpm not found`
- 4 min: `rsync not found; installer requires it`
- `No Chrome browser in container`

Attempt 2:

- 0.2 min: `rolldown native binding @rolldown/binding-linux-x64-gnu not auto-installed by pnpm (optional dependency was skipped)`
- 0.1 min: `missing 'unrun' package required by tsdown build config`
- 1.5 min: `system Node.js v18 is too old (requires v22+ for parseEnv, v23+ for zstd); foundation dsh CLI has exitOverride Commander bug (output/version silently consumed)`
- 0.3 min: `pnpm 11 requires Node 22.13+, pnpm 10 also requires Node 22.13+; pnpm 9 works`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
