# azure-devops-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/azure-devops-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/azure-devops-mcp

## Pinned environment

- Project commit: `52072ff41bb8849af9f19a85a260aa1b52824158`
- Test commit: `52072ff41bb8849af9f19a85a260aa1b52824158`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 3.1 | 1 | 1 | [run](https://argusic.com/run/bda6f15d-4639-4017-8f40-3aa8fa7ee3e5) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 is too old (project requires >=20), causing engine warnings and preventing optional dependency @azure/msal-node-extensions from resolving`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
