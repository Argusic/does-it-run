# ros-mcp-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/robotmcp/ros-mcp-server, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ros-mcp-server

## Pinned environment

- Project commit: `476591ac058f58cae810cc775e50b51f8d3d757c`
- Test commit: `476591ac058f58cae810cc775e50b51f8d3d757c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 59.7 to 59.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 50 | 59.7 | 5 | 5 | [run](https://argusic.com/run/777e6104-959f-4a47-a6fb-4e1b9d4284ee) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Python externally managed (PEP 668)`
- 1 min: `setuptools/wheel not in fresh venv`
- 45 min: `pip install -e .[dev] timed out downloading all deps at once`
- 5 min: `mcp 2.3.0 missing deps (opentelemetry-api, pyjwt, python-multipart)`
- 10 min: `Docker not available , integration tests skipped`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
