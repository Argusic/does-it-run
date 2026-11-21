# seonaut

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/StJudeWasHere/seonaut, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/seonaut

## Pinned environment

- Project commit: `880b312c28fab8b0bf7fe4f9449dc4746dbb82ff`
- Test commit: `880b312c28fab8b0bf7fe4f9449dc4746dbb82ff`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8.6 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 8.6 | 3 | 3 | [run](https://argusic.com/run/4e0a49a2-64cb-4eba-9970-1ed847c1d85c) |
| 2 | pass with mocks | 92 | 8 | 9.8 | 2 | 2 | [run](https://argusic.com/run/d911f3d5-48dc-4034-b7b7-8d8423643711) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Go toolchain and Docker/MySQL not present in container (no root to apt install)`
- 1 min: `First mariadbd nohup start exited before InnoDB finished initializing`
- 1 min: `Backgrounded 'go run' server died when the harness reaped the backgrounded process group`

Attempt 2:

- 2 min: `Go not installed in container`
- 5 min: `MySQL database not available (config pointed to hostname 'db')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
