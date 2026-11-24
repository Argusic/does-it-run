# home-assistant-vibecode-agent

**Verdict: runs with mocks.** Argusic Score 88.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Coolver/home-assistant-vibecode-agent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/home-assistant-vibecode-agent

## Pinned environment

- Project commit: `d361f865b42f95f1136503820cbb0d6555dedac8`
- Test commit: `d361f865b42f95f1136503820cbb0d6555dedac8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 6.8 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 10.1 | 2 | 2 | [run](https://argusic.com/run/121a9eea-6967-4fd0-9974-b10afc9d5ad8) |
| 2 | pass with mocks | 85.33 | 9 | 6.8 | 3 | 2 | [run](https://argusic.com/run/aeee1b60-1c78-4a50-a89b-ed1b1e54e78b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `httpx 1.x incompatible with starlette TestClient , pytest collection failed with TypeError: Client.__init__() got an unexpected keyword argument 'app'`
- 3 min: `except Exception in app/api/hacs.py:480 caught HTTPException(400) from HACS-not-installed check and re-wrapped it as 500, causing test_json_body_is_not_query_validation_error to fail`

Attempt 2:

- 2 min: `HTTPException in install_hacs_repository caught by generic except clause, re-raised as 500`
- 1 min: `httpx 0.28 removed 'app' param from Client.__init__ breaking Starlette TestClient`
- `3 MCP schema tests require external /work/home-assistant-mcp TS repo not present in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
