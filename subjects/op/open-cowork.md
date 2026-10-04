# open-cowork

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenCoworkAI/open-cowork, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-cowork

## Pinned environment

- Project commit: `a1d0e4ab0f0f78bc42c622653174650cd2025968`
- Test commit: `a1d0e4ab0f0f78bc42c622653174650cd2025968`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 63 to 63 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 63 | 3 | 3 | [run](https://argusic.com/run/68fcb19b-bdbe-485a-9a70-5eedee5d27a1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js <22 in container (18.19.1), project requires >=22`
- 0.5 min: `better-sqlite3 native module ABI mismatch after node upgrade`
- 2 min: `MCP protocol tests timeout because dist-mcp bundle not built`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
