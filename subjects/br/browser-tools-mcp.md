# browser-tools-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AgentDeskAI/browser-tools-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/browser-tools-mcp

## Pinned environment

- Project commit: `99acee8d02f12f6e64dc7f33608bb34427ce90c7`
- Test commit: `99acee8d02f12f6e64dc7f33608bb34427ce90c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.9 to 11.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.7 | 11.9 | 1 | 1 | [run](https://argusic.com/run/ae7bec8c-4552-4e81-84c1-6ba031cf4021) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Integration test 'still produces a usable client when the connector cannot start' failed because port 1 was not privileged in this container (the test assumed EACCES, but the runner user can bind low ports).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
