# E2B

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/e2b-dev/E2B, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/e2b

## Pinned environment

- Project commit: `ccaf9fc0ffe6ac39c7ec786af7608ab1de19467b`
- Test commit: `ccaf9fc0ffe6ac39c7ec786af7608ab1de19467b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 33 to 33 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 33 | 33 | 3 | 3 | [run](https://argusic.com/run/8bc7c243-c865-48db-9424-94cd2f6d5128) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pnpm not on PATH (node v18.19.1 bundled)`
- 1 min: `uv not installed`
- `No E2B_API_KEY in environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
