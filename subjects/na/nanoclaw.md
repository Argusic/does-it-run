# nanoclaw

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nanocoai/nanoclaw, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nanoclaw

## Pinned environment

- Project commit: `c313d061b0263dfbb1967ab64e4d7524c09a71a0`
- Test commit: `c313d061b0263dfbb1967ab64e4d7524c09a71a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 9.9 to 50.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.9 | 4 | 4 | [run](https://argusic.com/run/d05f4245-cb0f-48fa-b07e-de35afc0e557) |
| 2 | pass with mocks | 92 | 51 | 50.9 | 3 | 3 | [run](https://argusic.com/run/ee797e04-31ac-4e9a-9c3d-7d685852eb8b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node 18 too old (project requires >=22) - better-sqlite3 prebuilt binary segfaulted`
- 1 min: `@rolldown/binding-linux-x64-gnu native binding missing for vitest`
- 1 min: `better-sqlite3 build script blocked by pnpm onlyBuiltDependencies`
- `pnpm not found initially`

Attempt 2:

- 5 min: `System Node.js 18 is too old for vitest 4.x (needs >=22). pnpm install warned about unsupported engine, vitest crashed with SyntaxError on node:util.styleText`
- 20 min: `better-sqlite3 prebuilt binary (compiled for Node 18 ABI modules=109) segfaulted on Node 22 (modules=127). Rebuild from source using force_build=1 also linked against system libnode.so.109 instead of self-contained N-API. Manual g++ compila`
- `process.chdir() not supported in vitest thread workers , 12 config-webhook-port tests failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
