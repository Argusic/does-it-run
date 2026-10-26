# moai-cowork

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modu-ai/moai-cowork, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/moai-cowork

## Pinned environment

- Project commit: `6bc6098ae963dae0679daaa39fc40316355bdb13`
- Test commit: `6bc6098ae963dae0679daaa39fc40316355bdb13`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.5 to 2.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 2.5 | 1 | 1 | [run](https://argusic.com/run/14dcbf20-5994-4e94-a184-97849b70496d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `moai-mcp-smartstore dev dependencies (pytest, pytest-asyncio, requests-mock) not installed by default uv sync`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
