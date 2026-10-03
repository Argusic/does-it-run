# fastmcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PrefectHQ/fastmcp, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/run/ffbfa502-96c3-4440-b43c-0539d5b6f758

## Pinned environment

- Project commit: `75d50ffb683ba502e86bf833411c46234749270b`
- Test commit: `75d50ffb683ba502e86bf833411c46234749270b`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 40.9 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/ffbfa502-96c3-4440-b43c-0539d5b6f758) |
| 1 | pass with mocks | 92 | 3 | 40.9 | 5 | 5 | [run](https://argusic.com/run/3255003d-8bff-4bbd-9b5a-395dd1081ee4) |
| 2 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/fcd62e74-d95e-4559-b48a-1fe1d5320ba3) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `uv not installed , missing from PATH`
- 5 min: `pytest-xdist hangs , worker subprocess deadlock with pytest 9.1.1 + xdist 3.8.0`
- 5 min: `python not on PATH , stdio subprocess tests fail with 'No such file or directory: python'`
- 2 min: `uv not on PATH , uv transport tests fail with 'No such file or directory: uv'`
- 2 min: `MCP conformance tests require Node.js >=20 but container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
