# docs-mcp-server

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arabold/docs-mcp-server, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/docs-mcp-server

## Pinned environment

- Project commit: `f2938c47bb8937c650f0d5ddb614f867773b29f4`
- Test commit: `f2938c47bb8937c650f0d5ddb614f867773b29f4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.9 | 3 | 3 | [run](https://argusic.com/run/fd190ee8-8fb7-4ba2-bbae-97e0b584044f) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node v18 too old, project needs 22+`
- 1 min: `rolldown native binding not installed by npm`
- 3 min: `rolldown 1.1.5 API incompatible with Node 22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
