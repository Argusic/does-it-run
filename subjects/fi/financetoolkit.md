# FinanceToolkit

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JerBouma/FinanceToolkit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/financetoolkit

## Pinned environment

- Project commit: `9fa19f9e97fee229dad4d65cf9c1448597af5df5`
- Test commit: `9fa19f9e97fee229dad4d65cf9c1448597af5df5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 27.5 to 37.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 37.2 | 0 | 0 | [run](https://argusic.com/run/36f5dedc-6b5d-4578-ac71-e610267c0427) |
| 2 | fail | 80 | 4 | 27.5 | 5 | 5 | [run](https://argusic.com/run/096528cf-c82a-479f-a671-b8d553f86459) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `ImportError: No module named 'mcp.server.fastmcp' - FastMCP moved to separate package in mcp 2.x`
- 1 min: `TypeError: FastMCP() no longer accepts log_level/host kwargs`
- 2 min: `TypeError: FastMCP.add_tool() got unexpected keyword args (name, description)`
- 1 min: `AttributeError: FastMCP object has no attribute 'sse_app'`
- 2 min: `test_build_mcp_app_uses_global_cache_path failed: test stubs mcp.server.fastmcp but code now imports from fastmcp`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
