# mcp-server-kubernetes

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Flux159/mcp-server-kubernetes, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcp-server-kubernetes

## Pinned environment

- Project commit: `3d71add204014dcceddebe53e9695ed7d8a6d129`
- Test commit: `3d71add204014dcceddebe53e9695ed7d8a6d129`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 14.2 to 55.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 14.2 | 2 | 2 | [run](https://argusic.com/run/8b4e6a25-e4fe-4c8f-ad5a-409488945023) |
| 2 | pass with mocks | 92 | 1 | 55.1 | 3 | 3 | [run](https://argusic.com/run/28d9cb29-bb92-45b2-bfe9-87dd90e8971f) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `bun not available in PATH`
- 3 min: `kubectl not installed; official CDN download returned 404 errors`

Attempt 2:

- 1 min: `kubectl binary not found in PATH`
- 1 min: `bun binary not found in PATH`
- 15 min: `No Kubernetes cluster available for integration tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
