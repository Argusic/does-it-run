# sponge

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-dev-frame/sponge, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/sponge

## Pinned environment

- Project commit: `beef9eecdc5e2dc6b1358f130d8e9133771c277b`
- Test commit: `beef9eecdc5e2dc6b1358f130d8e9133771c277b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.9 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 23.9 | 2 | 2 | [run](https://argusic.com/run/2dc56ca9-12fd-45c9-a0af-1a142c10f3d0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go (golang) not installed in container`
- 2 min: `protoc binary not installed by sponge init`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
