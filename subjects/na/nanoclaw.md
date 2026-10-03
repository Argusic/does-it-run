# nanoclaw

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nanocoai/nanoclaw, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nanoclaw

## Pinned environment

- Project commit: `c313d061b0263dfbb1967ab64e4d7524c09a71a0`
- Test commit: `c313d061b0263dfbb1967ab64e4d7524c09a71a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.9 | 4 | 4 | [run](https://argusic.com/run/d05f4245-cb0f-48fa-b07e-de35afc0e557) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node 18 too old (project requires >=22) - better-sqlite3 prebuilt binary segfaulted`
- 1 min: `@rolldown/binding-linux-x64-gnu native binding missing for vitest`
- 1 min: `better-sqlite3 build script blocked by pnpm onlyBuiltDependencies`
- `pnpm not found initially`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
