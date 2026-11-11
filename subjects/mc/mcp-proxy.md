# mcp-proxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sparfenyuk/mcp-proxy, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-proxy

## Pinned environment

- Project commit: `153a96a61fde2bf5a23961c64a3dd96b5e385108`
- Test commit: `153a96a61fde2bf5a23961c64a3dd96b5e385108`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.9 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.2 | 1 | 1 | [run](https://argusic.com/run/23ca4565-c187-4577-b97f-d948c5787c55) |
| 2 | pass | 100 | 0.17 | 2.9 | 2 | 2 | [run](https://argusic.com/run/18be831a-6bea-4837-a671-e4e98129277d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Corrupted attr/exceptions.py with trailing null bytes causing SyntaxError on import`

Attempt 2:

- 2 min: `mcp>=1.27.1 constraint in pyproject.toml resolves to mcp 2.3.0 which has breaking API changes (removed request_ctx, renamed streamablehttp_client, removed create_connected_server_and_client_session, renamed McpError to MCPError)`
- 1 min: `mcp-reverse-proxy entry point references mcp_proxy.__main__:client but no client() function exists in __main__.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
