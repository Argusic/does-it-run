# ha-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/homeassistant-ai/ha-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ha-mcp

## Pinned environment

- Project commit: `58e31c7176fa4ad3358704e40c555bd3dc0f36c9`
- Test commit: `58e31c7176fa4ad3358704e40c555bd3dc0f36c9`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 4; wall time 42.2 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.2 | 0 | 0 | [run](https://argusic.com/run/c6a81747-1c5f-4d0d-b813-53d9c4d4f53d) |
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/e41e8275-3d14-405a-b2a3-35c09c079440) |
| 2 | timeout | none | n/a | 42.2 | 0 | 0 | [run](https://argusic.com/run/30568af7-aec3-433c-b827-7b4958d8eebd) |
| 2 | pass with mocks | 92 | 7 | 70.5 | 1 | 1 | [run](https://argusic.com/run/0100a87d-9ccb-4dbf-ae49-775e0bd21840) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `git submodule 'skills-vendor' not initialized , caused 3 test_helper_response_shape tests to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
