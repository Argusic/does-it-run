# supabase-mcp-server

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alexander-zuev/supabase-mcp-server, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/supabase-mcp-server

## Pinned environment

- Project commit: `bca07008fe46cae791221c2ee30df034c963ec56`
- Test commit: `bca07008fe46cae791221c2ee30df034c963ec56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13.8 to 66.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 66.3 | 0 | 0 | [run](https://argusic.com/run/1d347469-eaf0-46f1-b325-0c9695939135) |
| 2 | pass | 100 | 3 | 13.8 | 3 | 3 | [run](https://argusic.com/run/89a26e9a-60b2-45f8-bd92-6410fc5db787) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `pytest failed to start: pyproject.toml uses both [tool.pytest] and [tool.pytest.ini_options] simultaneously`
- 3 min: `ImportError: No module named 'mcp.server.fastmcp' because pip resolved mcp 2.3.0 which removed the FastMCP v1 API`
- 4 min: `test_comprehensive_spec_retrieval failed: fresh ApiSpecManager fetched the live remote spec (147 schemas) which lacks FunctionResponse, while the bundled fallback spec has it`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
