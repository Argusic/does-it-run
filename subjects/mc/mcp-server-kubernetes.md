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
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 14.2 | 2 | 2 | [run](https://argusic.com/run/8b4e6a25-e4fe-4c8f-ad5a-409488945023) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `bun not available in PATH`
- 3 min: `kubectl not installed; official CDN download returned 404 errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
