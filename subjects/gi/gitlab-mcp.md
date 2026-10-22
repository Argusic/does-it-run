# gitlab-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zereight/gitlab-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/gitlab-mcp

## Pinned environment

- Project commit: `95edb4901e7dfa1b6d35b6e48548a0b782521ac9`
- Test commit: `95edb4901e7dfa1b6d35b6e48548a0b782521ac9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 22 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20.1 | 22 | 1 | 1 | [run](https://argusic.com/run/846b26cf-def1-48e3-96b8-56c05c176de8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 was installed but package requires >=20 (from @hono/node-server dependency). npm install failed with EBADENGINE.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
