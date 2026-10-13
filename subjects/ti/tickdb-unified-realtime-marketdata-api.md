# tickdb-unified-realtime-marketdata-api

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TickDB/tickdb-unified-realtime-marketdata-api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tickdb-unified-realtime-marketdata-api

## Pinned environment

- Project commit: `37b2d3c13034f436e8a7aaa8fbd678888c38f46f`
- Test commit: `37b2d3c13034f436e8a7aaa8fbd678888c38f46f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.2 | 2 | 2 | [run](https://argusic.com/run/3806653e-f171-437e-888c-79b4e7c8482f) |

## What was observed on a clean machine

Attempt 1:

- `externally-managed-environment blocked pip install`
- 1 min: `mcp package resolved to v2.3.0 which broke FastMCP import`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
