# inference-gateway

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/inference-gateway/inference-gateway, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/inference-gateway

## Pinned environment

- Project commit: `97fe89fbe7c5abf5b9d77b092c1f9db4ed1c6538`
- Test commit: `97fe89fbe7c5abf5b9d77b092c1f9db4ed1c6538`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 12.3 | 3 | 3 | [run](https://argusic.com/run/9d55f840-cdc8-42f3-9440-eb94478f07fb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `sudo: command not found (install.sh always tries sudo mv; no root in container)`
- 1 min: `go: not found`
- 1 min: `task: not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
