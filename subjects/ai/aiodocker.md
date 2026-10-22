# aiodocker

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aio-libs/aiodocker, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/aiodocker

## Pinned environment

- Project commit: `178d8a0fc9fa49dfb737d94f9e3be0f3d3ddce04`
- Test commit: `178d8a0fc9fa49dfb737d94f9e3be0f3d3ddce04`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 1.6 to 21.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.5 | 1.6 | 0 | 0 | [run](https://argusic.com/run/e3b1536a-b494-4a75-929c-f07d0f21dfd9) |
| 2 | pass with mocks | 92 | 16 | 21.3 | 4 | 4 | [run](https://argusic.com/run/3b75d671-ab7d-44bb-9b9e-110eebf2112f) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `uv not available (not in PATH)`
- 1 min: `docker CLI not installed in container`
- 6 min: `Docker daemon cannot start (no root permissions, no user namespaces for rootless mode)`
- 2 min: `Tests that use Docker multiplexed streaming protocol (containers, images, execs, testcontainers) or docker subprocess (configs, secrets, swarm, nodes, services, dind) cannot run against mock`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
