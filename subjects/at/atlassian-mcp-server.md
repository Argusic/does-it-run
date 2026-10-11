# atlassian-mcp-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/atlassian/atlassian-mcp-server, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/atlassian-mcp-server

## Pinned environment

- Project commit: `eb9a5956a7ac6380c731c725a8382da53ad6d980`
- Test commit: `eb9a5956a7ac6380c731c725a8382da53ad6d980`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 3.8 | 2 | 2 | [run](https://argusic.com/run/ab02134a-9a15-4798-8abb-9fdd86315625) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Real endpoint https://mcp.atlassian.com/v2/mcp answered HTTP 401 with an OAuth WWW-Authenticate challenge (real Atlassian credentials required to proceed)`
- 1 min: `My mock-server setup accidentally truncated scripts/validation/test-helpers.mjs to an empty file`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
