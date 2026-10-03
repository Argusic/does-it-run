# awesome-agentic-ai-zh

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WenyuChiou/awesome-agentic-ai-zh, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/awesome-agentic-ai-zh

## Pinned environment

- Project commit: `dce3048e1f9ff328f6d155fff075a06d44665f81`
- Test commit: `dce3048e1f9ff328f6d155fff075a06d44665f81`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.2 to 21.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 21.2 | 8 | 8 | [run](https://argusic.com/run/ca6faf93-fd05-4963-a020-e04f34f4331c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `python3 pip not installed initially`
- `venv unavailable, needed --break-system-packages for pip installs`
- 1 min: `pytest not installed (6 test scripts failing)`
- 2 min: `missing numpy, chromadb for stage-6 tests`
- 1 min: `missing fastapi, uvicorn, httpx for stage-7/05-deploy test`
- 1 min: `missing langgraph for stage-4/01 and stage-4/03 tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
