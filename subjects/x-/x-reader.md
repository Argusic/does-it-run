# x-reader

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/runesleo/x-reader, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/x-reader

## Pinned environment

- Project commit: `8c79a611e686b3272aece70f09e70831b7912a77`
- Test commit: `8c79a611e686b3272aece70f09e70831b7912a77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 9.8 | 3 | 3 | [run](https://argusic.com/run/6be5b2f9-6cfa-4100-af0a-13521c11d7d5) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `UnifiedInbox.save() crashed with FileNotFoundError when inbox directory did not exist`
- 7 min: `Twitter Playwright tier failed after documented 'playwright install chromium' because channel="chrome" is hardcoded and system Chrome is absent; bundled Chromium also missing until installed`
- 16 min: `MCP --transport sse served bare Starlette with no SSE routes (POST /mcp -> 404); README documents only /mcp`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
