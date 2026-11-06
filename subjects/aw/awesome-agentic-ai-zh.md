# awesome-agentic-ai-zh

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WenyuChiou/awesome-agentic-ai-zh, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/awesome-agentic-ai-zh

## Pinned environment

- Project commit: `dce3048e1f9ff328f6d155fff075a06d44665f81`
- Test commit: `dce3048e1f9ff328f6d155fff075a06d44665f81`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.4 to 21.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 21.2 | 8 | 8 | [run](https://argusic.com/run/ca6faf93-fd05-4963-a020-e04f34f4331c) |
| 2 | pass with mocks | 92 | 1 | 7.4 | 2 | 2 | [run](https://argusic.com/run/711836ed-7601-4bfc-9980-252c44d1926d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `python3 pip not installed initially`
- `venv unavailable, needed --break-system-packages for pip installs`
- 1 min: `pytest not installed (6 test scripts failing)`
- 2 min: `missing numpy, chromadb for stage-6 tests`
- 1 min: `missing fastapi, uvicorn, httpx for stage-7/05-deploy test`
- 1 min: `missing langgraph for stage-4/01 and stage-4/03 tests`

Attempt 2:

- 2 min: `pip install opencc-python-reimplemented missing for scripts/test_hans_chars.py , 13 test failures`
- 3 min: `pip install pydantic-ai, chromadb, fastapi, smolagents missing for example tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
