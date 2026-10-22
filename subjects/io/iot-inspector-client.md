# iot-inspector-client

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nyu-mlab/iot-inspector-client, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/iot-inspector-client

## Pinned environment

- Project commit: `cae56e6e890f7839edd84e382f72cadbb5add2ef`
- Test commit: `cae56e6e890f7839edd84e382f72cadbb5add2ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 28 | 10 | 3 | 3 | [run](https://argusic.com/run/237dc67e-0ed0-45ae-8896-9e132949655a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pytest not declared in pyproject.toml/uv.lock`
- 2 min: `iot_inspector console script fails: ModuleNotFoundError No module named 'page_manager'`
- 10 min: `packet_collector exits unless MongoDB is reachable (no mongod in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
