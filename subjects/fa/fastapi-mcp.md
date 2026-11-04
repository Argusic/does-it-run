# fastapi_mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tadata-org/fastapi_mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fastapi-mcp

## Pinned environment

- Project commit: `e5cad13cabfc725bbcb047e526816d887d96da62`
- Test commit: `e5cad13cabfc725bbcb047e526816d887d96da62`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.4 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 5.4 | 3 | 3 | [run](https://argusic.com/run/b9a5638d-7fa5-4d2e-a8b2-3272c098c43c) |
| 2 | pass | 100 | 12 | 9.7 | 1 | 1 | [run](https://argusic.com/run/5812ed51-cebb-4017-8671-171c170927cb) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Pip install failed due to externally-managed-environment (PEP 668)`
- 1 min: `Installed mcp 2.2.0 (latest) but the project's lock file pins mcp 1.12.1 and the tests use the v1 API`
- 0.3 min: `Dev extras not installed by pip (pytest etc missing)`

Attempt 2:

- 4 min: `mcp>=1.12.0 in pyproject.toml allows mcp 2.x which has a completely different API (Server.__init__ signature changed, list_tools/call_tool decorators removed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
