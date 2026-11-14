# mcptools

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/f/mcptools, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mcptools

## Pinned environment

- Project commit: `e7bd7246118384095ba22fd219ff38a1bf1cb792`
- Test commit: `e7bd7246118384095ba22fd219ff38a1bf1cb792`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.1 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 13 | 0 | 0 | [run](https://argusic.com/run/b891ae49-b7a6-4f90-afb8-81d92a9d308c) |
| 2 | pass | 100 | 0.5 | 1.1 | 1 | 1 | [run](https://argusic.com/run/4fe36e38-f9af-4e57-b8fc-067429aa6cfe) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Go not installed in container (no root to apt-get)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
