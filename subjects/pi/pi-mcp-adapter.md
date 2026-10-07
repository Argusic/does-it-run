# pi-mcp-adapter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nicobailon/pi-mcp-adapter, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-mcp-adapter

## Pinned environment

- Project commit: `7bf2332932b652416ea717e154352baed7420b66`
- Test commit: `7bf2332932b652416ea717e154352baed7420b66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.6 to 8.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 8.6 | 1 | 1 | [run](https://argusic.com/run/266bd84f-ed6b-4fc4-83ef-ae6700089f5e) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node 18.19.1 installed system-wide, but project requires Node >=20 (crypto global missing, import 'with' JSON syntax unsupported)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
