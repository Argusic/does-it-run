# ref-tools-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ref-tools/ref-tools-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ref-tools-mcp

## Pinned environment

- Project commit: `83970a35627785a0589ae2dbe5510b4a3dd04146`
- Test commit: `83970a35627785a0589ae2dbe5510b4a3dd04146`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 2.9 | 3 | 3 | [run](https://argusic.com/run/48b0ed69-8dc6-45e6-8a50-9d14dcd87eef) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Background mock/server processes terminated when their launching shell session ended`
- 2 min: `Python urllib connected to localhost over IPv6, getting EADDRNOTAVAIL against the IPv4 HTTP listener`
- 1 min: `Test client crashed on MCP notifications/initialized empty 202 response`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
