# FlowX

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AIpRoBuilder/FlowX, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/flowx

## Pinned environment

- Project commit: `212a78e84d805c909d983cfc91dda0d9c38b62d9`
- Test commit: `212a78e84d805c909d983cfc91dda0d9c38b62d9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.9 to 34.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 38 | 34.9 | 8 | 8 | [run](https://argusic.com/run/84ee9132-4ca3-4d5e-b4db-f9fd9c1c69d5) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `pip install -e . failed building pydaograph: Python development headers (Python.h) not found under /usr/include/python3.12; no prebuilt wheel on PyPI and no root to install python3-dev.`
- 3 min: `flowx-mcp tools/call list_workflows failed with 'Missing DEEPSEEK_API_KEY' when started from the README's .env.example; engine-backed tools require a provider API key at startup.`
- 12 min: `run_service launched the generated main.py with /usr/bin/python3 because select_python_command picked PATH python instead of the FlowX venv; the service crashed with ModuleNotFoundError: No module named 'dotenv' and base_url never answered.`
- 18 min: `flowx-a2a served GET /.well-known/agent-card.json and POST /a2a as 422 'missing query request': Request was imported only inside create_app while 'from __future__ import annotations' made FastAPI resolve it in module globals.`
- 10 min: `A2A message/send with metadata.workflowId was rejected with 'a new workflow needs a requirement' because every message was regrouped through build_workflow; README promised the left-out continuation path.`
- 8 min: `flowx-mcp over stdio emitted non-JSON lines (uvicorn 'INFO ... GET / HTTP/1.1 200 OK') on the stdout protocol channel after run_service/run_step, breaking clients.`
- 5 min: `Global pip resolution was not clean (sse-starlette requires starlette>=0.49.1); during diagnosis I exercised fastapi 0.115.14/starlette 0.46.2 and the A2A failure reproduced identically, confirming it was not a version artifact.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
