# electric-pglite

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/electric-sql/electric-pglite, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/fa0ad0d6-a78f-4407-935a-02e5274454ba

## Pinned environment

- Project commit: `dbd6eb41c9aca5b655adf0f516c3c9888469a02c`
- Test commit: `dbd6eb41c9aca5b655adf0f516c3c9888469a02c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 33 | 8.5 | 4 | 2 | [run](https://argusic.com/run/fa0ad0d6-a78f-4407-935a-02e5274454ba) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 instead of required >=20 - used successfully anyway`
- 2 min: `pnpm not installed system-wide - installed via npm locally`
- 3 min: `Docker not available for WASM build - had to download pre-built binaries from npm`
- 1 min: `pglite-age extension failed to build - missing AGE WASM binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
