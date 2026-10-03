# blender-mcp

**Verdict: runs.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ahujasid/blender-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/blender-mcp

## Pinned environment

- Project commit: `5866814479b4e2ca674d8d44969a9a2a78fdc8bb`
- Test commit: `5866814479b4e2ca674d8d44969a9a2a78fdc8bb`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 2.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.2 | 4.4 | 1 | 0 | [run](https://argusic.com/run/3f36636d-544d-40ec-a2b3-2e82f36a2e26) |
| 2 | pass with mocks | 92 | 3.2 | 2.6 | 0 | 0 | [run](https://argusic.com/run/72b7c896-557b-46b9-a1a2-42bd8c201474) |
| 3 | pass with mocks | 92 | 2 | 2.4 | 0 | 0 | [run](https://argusic.com/run/605facd6-411c-44d0-ad65-821d66ece12c) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
