# MiroThinker

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MiroMindAI/MiroThinker, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mirothinker

## Pinned environment

- Project commit: `1c4253f6774bf40314271a827304b842100e054c`
- Test commit: `1c4253f6774bf40314271a827304b842100e054c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.6 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 11.6 | 1 | 1 | [run](https://argusic.com/run/5622df2f-e659-4666-a965-a5f5118e01b1) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `miroflow-tools resolved mcp>=2 / fastmcp>=4 (v2 API), but code uses FastMCP from v1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
