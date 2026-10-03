# grist-core

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gristlabs/grist-core, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/grist-core

## Pinned environment

- Project commit: `298d4661ce3513a6a459c5441f9c5baea4356cc8`
- Test commit: `298d4661ce3513a6a459c5441f9c5baea4356cc8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 31.8 to 47.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 32 | 47.8 | 5 | 5 | [run](https://argusic.com/run/bdd31497-e69a-4ef3-8139-7e84b8b8619f) |
| 2 | pass | 100 | 10 | 31.8 | 5 | 5 | [run](https://argusic.com/run/bfbe0673-cb66-4f0a-a400-2e3e2c11f339) |
| 3 | pass | 100 | 37 | 38.2 | 1 | 1 | [run](https://argusic.com/run/1ac14b6a-467f-41f4-9a6f-a10e03d6130c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `TypeScript compiler (tsc) not found on PATH during build`
- 0.5 min: `webpack.check.js uses ESM import syntax, not supported by Node 18 CJS runner`
- 8 min: `ESM-only packages (uuid, file-type, boxen, p-limit) cannot be require()'d in Node 18`
- `sqlite3 CLI binary not available for tests that spawn it`
- `Python 3.12 compatibility warnings for deprecated ast.Str in astroid`

Attempt 2:

- 2 min: `Node v18 was incompatible with @gristlabs/sqlite3 (needs >=20.17.0)`
- 1 min: `yarn not found on PATH`
- 1 min: `generateInitialDocSql test failed: SQL schema file was out of date`
- `Sandbox/Pyodide tests fail: 'npm deno package not found'`
- `Comm test 'should order server messages correctly with failedSend before close' failed: got 'close' expected 'failedSend'`

Attempt 3:

- 5 min: `System Node.js v18.19.1 too old for project's dependencies (requires >=20.17.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
