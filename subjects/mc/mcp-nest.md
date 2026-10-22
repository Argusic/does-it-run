# MCP-Nest

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rekog-labs/MCP-Nest, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcp-nest

## Pinned environment

- Project commit: `3c5531dc3f5634fc5ec784f3ca27b66ee3e34b4c`
- Test commit: `3c5531dc3f5634fc5ec784f3ca27b66ee3e34b4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.1 to 12.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 12.1 | 1 | 1 | [run](https://argusic.com/run/43f12865-1467-4100-90cb-dcefa3833ce4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not found in container; required by build and test scripts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
