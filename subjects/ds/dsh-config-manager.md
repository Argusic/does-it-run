# dsh-config-manager

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xiajiajun516/dsh-config-manager, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-config-manager

## Pinned environment

- Project commit: `5bca520674d13c355b26b85296c15a214201dc91`
- Test commit: `5bca520674d13c355b26b85296c15a214201dc91`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.8 to 26.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 26.8 | 5 | 5 | [run](https://argusic.com/run/d221d66d-28d1-40db-9434-9b5577156641) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 too old (requires ^22.19.0 || >=24.0.0)`
- 1 min: `pnpm install --ignore-scripts skipped optional native binding @rolldown/binding-linux-x64-gnu needed by tsdown`
- 1 min: `tsdown required unrun package not in dependencies`
- `TypeScript typecheck has known conflict TS2717 in chat-slots.ts (SessionId vs string from DSH session types), build tsconfig excludes client dir`
- `2 pre-existing test failures (MC-5 retention boundary and fork-reconcile timeout)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
