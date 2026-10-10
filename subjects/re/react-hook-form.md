# react-hook-form

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/react-hook-form/react-hook-form, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-hook-form

## Pinned environment

- Project commit: `e76876b02550b3ad48a351c638845d9dc1aaa3c8`
- Test commit: `e76876b02550b3ad48a351c638845d9dc1aaa3c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.3 to 20.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 20.3 | 4 | 4 | [run](https://argusic.com/run/ea0367aa-9d5f-4d9e-8127-3a81d79d9003) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pnpm not present and pnpm 9/11 rejected the workspace's pnpm-workspace.yaml lacking a 'packages' field (CI expects pnpm 11 on Node 22)`
- 4 min: `App 'pnpm build' failed: src/types/path/index.ts re-exports types without 'export type', error TS1205 under app's isolatedModules`
- 5 min: `App 'pnpm build' still fails on pre-existing demo type errors (joi Buffer, resolver mismatches, changeInputType indexing) even with app's pinned TypeScript 5.7.2; vite build itself succeeds`
- 5 min: `e2e 'pnpm e2e' first run was OOM-killed (exit 137) from 90 parallel browser workers (4 CPU / 8GB container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
