# daydreams

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/daydreamsai/daydreams, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/daydreams

## Pinned environment

- Project commit: `e3231c3de1082114162a7432aa1a468bcbc04c7e`
- Test commit: `e3231c3de1082114162a7432aa1a468bcbc04c7e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.3 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.3 | 3 | 3 | [run](https://argusic.com/run/2e446b4a-f36f-4000-b5fe-f165fdb3e76d) |
| 2 | pass | 100 | 2 | 7.8 | 1 | 1 | [run](https://argusic.com/run/ed24c5f0-fdf8-4b12-80cb-828d7805ede1) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 2 min: `pnpm install ERR_PNPM_IGNORED_BUILDS for @coinbase/x402, bigint-buffer, keccak`
- 2 min: `Missing dist/ for discord, hyperliquid, mongo packages`

Attempt 2:

- 2 min: `pnpm ERR_PNPM_IGNORED_BUILDS: ignoredBuildDependencies in pnpm-workspace.yaml not recognized by pnpm v12, blocking install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
