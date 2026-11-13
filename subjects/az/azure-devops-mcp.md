# azure-devops-mcp

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/azure-devops-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/azure-devops-mcp

## Pinned environment

- Project commit: `52072ff41bb8849af9f19a85a260aa1b52824158`
- Test commit: `52072ff41bb8849af9f19a85a260aa1b52824158`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.1 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 3.1 | 1 | 1 | [run](https://argusic.com/run/bda6f15d-4639-4017-8f40-3aa8fa7ee3e5) |
| 2 | pass | 100 | 6 | 6.4 | 3 | 3 | [run](https://argusic.com/run/df5b611f-cce3-47ae-8759-45ecbc64099e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 is too old (project requires >=20), causing engine warnings and preventing optional dependency @azure/msal-node-extensions from resolving`

Attempt 2:

- 1 min: `TypeScript build error: Cannot find module '@azure/msal-node-extensions'`
- 3 min: `Jest test error: Cannot find module '@azure/msal-node-extensions' in pat-auth.test.ts`
- 2 min: `Runtime error: yargs@18 uses /v regex flag unsupported by Node.js 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
