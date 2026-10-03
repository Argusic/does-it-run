# MobileBuildMCP

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/getsentry/MobileBuildMCP, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mobilebuildmcp

## Pinned environment

- Project commit: `d13ff0c707b0681769cf31da0eb42c4f94ceafff`
- Test commit: `d13ff0c707b0681769cf31da0eb42c4f94ceafff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 4.9 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 4.9 | 1 | 1 | [run](https://argusic.com/run/479f218e-3294-418d-8bb7-c3961ed967f2) |
| 2 | pass | 100 | 33 | 5.6 | 2 | 2 | [run](https://argusic.com/run/d8bd78fa-70c1-4472-b837-c9880c77e1e1) |
| 3 | pass | 100 | 8 | 9.6 | 1 | 1 | [run](https://argusic.com/run/a68791a8-40e4-4e7e-9cbf-1e05adfe1bda) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Node 18.19.1 missing 'node:util.styleText' export required by vitest 4.x/rolldown`

Attempt 2:

- 2 min: `Node 18.19.1 too old for vitest/rolldown (requires export 'styleText' from node:util, added in Node 20)`
- 2 min: `Native binding missing after Node upgrade (rolldown @rolldown/binding-linux-x64-gnu not found)`

Attempt 3:

- 3 min: `Node.js 18 (system default) too old for vitest@4 rolldown native binding and yargs-parser@22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
