# ouroboros

**Verdict: runs with mocks.** Argusic Score 88.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Q00/ouroboros, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/60480488-3353-4b59-956c-9eb20800863a

## Pinned environment

- Project commit: `55aa1aa9871da13ab48c3c29b456c4aa73880c9f`
- Test commit: `55aa1aa9871da13ab48c3c29b456c4aa73880c9f`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 4; wall time 36.8 to 73 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 51.3 | 0 | 0 | [run](https://argusic.com/run/60480488-3353-4b59-956c-9eb20800863a) |
| 1 | pass with mocks | 85.33 | 1 | 36.8 | 3 | 2 | [run](https://argusic.com/run/6e9178be-63dc-42a2-8003-775c1665a4c7) |
| 2 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/6ba67dbf-4657-4cd7-baa3-5f66e16032ea) |
| 3 | pass with mocks | 92 | 3 | 73 | 1 | 1 | [run](https://argusic.com/run/47a345e3-55dc-45a8-b7b3-4840b8135115) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv package manager not preinstalled in container`
- 2 min: `pytest collection failed on 4 MCP tests: ModuleNotFoundError: No module named 'mcp' (mcp-test dependency group not in default dev sync)`
- 30 min: `Full pytest suite did not complete within remaining time budget; a parallel run (-n auto, excluding slow/performance markers) showed multiple F failures around 8-11% progress before the 45-minute mission time limit was reached`

Attempt 3:

- 2 min: `Two Windows path-capacity unit tests fail on Linux: expected_artifacts=("nested/" + "a" * 200,) does not exceed 260 UTF-16 units on Linux because os.path.realpath("C:\...") produces a different length`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
