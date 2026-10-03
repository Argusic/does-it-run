# jira-cli

**Verdict: runs with mocks.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ankitpokhrel/jira-cli, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/jira-cli

## Pinned environment

- Project commit: `11ec3f844ab282d88367ded20de548bb6629ee14`
- Test commit: `11ec3f844ab282d88367ded20de548bb6629ee14`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 3; wall time 2.1 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass with mocks | 92 | 13 | 14 | 3 | 3 | [run](https://argusic.com/run/331e3a4a-005b-464d-92e7-efc7cf77519c) |
| 2 | pass with mocks | 92 | 3 | 5 | 0 | 0 | [run](https://argusic.com/run/64840c20-fc75-4b21-8ef1-8e1e237ee310) |
| 3 | fail | 80 | 4 | 2.1 | 0 | 0 | [run](https://argusic.com/run/acad380d-3a05-45f2-a39e-3487a0024ba0) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go 1.26.8 not installed in container`
- 1 min: `make command not found`
- 1 min: `gcc not installed, CGO_ENABLED=1 -race tests fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
