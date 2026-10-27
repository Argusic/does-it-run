# facebook-ads-library-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RamsesAguirre777/facebook-ads-library-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/facebook-ads-library-mcp

## Pinned environment

- Project commit: `ea3c877855c16fb4594f640634d06f85e414eadb`
- Test commit: `ea3c877855c16fb4594f640634d06f85e414eadb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.7 | 1 | 1 | [run](https://argusic.com/run/2902955d-19db-4c63-a064-6d8d2ec9f479) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Print statement on stdout at line 287 (__main__ banner) broke MCP stdio JSON-RPC transport , the mcp client library failed to parse 'Facebook Ad Library MCP , scraping tools: ...' as JSON`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
