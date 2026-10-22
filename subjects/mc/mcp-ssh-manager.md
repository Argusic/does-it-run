# mcp-ssh-manager

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bvisible/mcp-ssh-manager, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mcp-ssh-manager

## Pinned environment

- Project commit: `0ec433a23834816b21ee313a0f264ec1e6ede565`
- Test commit: `0ec433a23834816b21ee313a0f264ec1e6ede565`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9 to 9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 12 | 9 | 2 | 1 | [run](https://argusic.com/run/42b53f75-c032-408a-84e0-29915db0d5f1) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `cli/install.sh fails: missing required system 'ssh' binary (container has no openssh-client, no root to install it; apt-get fails with Permission denied on dpkg lock)`
- 3 min: `MCP tools/list answered -32601 immediately after initialize (server registers tools only after configuration load); no code defect, my probe needed a startup delay before tools/call`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
