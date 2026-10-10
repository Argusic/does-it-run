# alook

**Verdict: runs.** Argusic Score 56.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alookai/alook, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/alook

## Pinned environment

- Project commit: `f29478da2daddeec05cf5ff0a20f501aecca4a58`
- Test commit: `f29478da2daddeec05cf5ff0a20f501aecca4a58`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 48.6 to 50.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 48.6 | 0 | 0 | [run](https://argusic.com/run/b31d85b5-e2a1-40a0-b141-731ef8681958) |
| 2 | pass | 93.33 | 15 | 50.8 | 6 | 4 | [run](https://argusic.com/run/894b7cba-ba38-4fce-92f3-0802f994b061) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Node.js v18 lacks styleText, node:sqlite, --experimental-websocket, --experimental-require-module`
- 2 min: `pnpm not installed at PATH`
- 8 min: `required optional native binding @rolldown/binding-linux-x64-gnu missing from lockfile install`
- 5 min: `better-sqlite3 native module compiled for wrong Node ABI`
- `bun not available (required for daemon packed tests: agent-driver-bundle and version.packed)`
- `apple-oauth-hardening test fails due to better-sqlite3/kysely adapter API mismatch (stmt.columns is not a function)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
