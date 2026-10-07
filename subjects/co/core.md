# core

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vuejs/core, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/core

## Pinned environment

- Project commit: `4ab865a848a1da3d10fb674f857e5fff13094644`
- Test commit: `4ab865a848a1da3d10fb674f857e5fff13094644`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 6.4 | 3 | 3 | [run](https://argusic.com/run/04f7133f-ac38-43ee-b80a-e938f6fdb440) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 is too old; Vue 3.5.43 requires >=20.0.0 and rolldown native binding requires ^20.19.0||>=22.12.0`
- 2 min: `pnpm not found after node switch; had to install it via npm with a custom prefix`
- 2 min: `Rolldown native binding @rolldown/binding-linux-x64-gnu was not fetched by pnpm due to engine version mismatch during initial install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
