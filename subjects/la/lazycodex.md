# lazycodex

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/code-yeongyu/lazycodex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lazycodex

## Pinned environment

- Project commit: `8d16365e3f2153582f46642f561f60656fd60b5b`
- Test commit: `8d16365e3f2153582f46642f561f60656fd60b5b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 36.8 to 36.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 8.5 | 36.8 | 3 | 2 | [run](https://argusic.com/run/bde52935-c6fe-4d4c-98fa-d7eaa9ab45ed) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npx lazycodex-ai install fails: oh-my-openagent-linux-x64 platform binary package lacks "type": "module" (Node 18 needs it for ES module imports)`
- 3 min: `npx lazycodex-ai install fails at final step: npm 9.x doesn't support workspace:* protocol (plugin source uses npm workspaces)`
- 1 min: `Plugin tests: 30/319 fail because @oh-my-opencode/shared-skills is not resolvable (npm install failed on workspace deps)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
