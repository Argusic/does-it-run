# Vibe-Trading

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HKUDS/Vibe-Trading, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vibe-trading

## Pinned environment

- Project commit: `899d3c7536a817ff418aefef934e81dfe60d179b`
- Test commit: `899d3c7536a817ff418aefef934e81dfe60d179b`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 18.9 to 62.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 18.9 | 3 | 3 | [run](https://argusic.com/run/ce56967a-b12a-48ff-aeb4-35240bd2fd40) |
| 2 | pass | 100 | 2.5 | 23.8 | 2 | 2 | [run](https://argusic.com/run/8b14f0ac-9b21-4c38-bbbb-9b4b608c0dc9) |
| 3 | pass with mocks | 92 | 0.5 | 62.3 | 1 | 1 | [run](https://argusic.com/run/709988ad-c91f-4cd7-9f90-790b9325bd4b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test_mcp_oauth_schema.py: _IBKROAuth (httpx2.Auth) not accepted by httpx.AsyncClient auth param`
- 2 min: `test_mcp_oauth_schema.py: read_timeout_seconds is now float, not timedelta`
- 2 min: `test_oauth_token_cache.py + test_mcp_client_adapter.py: McpError API changed to require positional code,message args`

Attempt 2:

- 5 min: `7 MCP-related tests failed: fastmcp 4.x / mcp-types 2.x broke McpError constructor, httpx Auth contract, and OAuth import paths`

Attempt 3:

- 2 min: `4 test failures due to fastmcp/mcp library version drift (pip resolved fastmcp 4.0.5 instead of lock file 3.4.6, mcp 2.2.0 instead of 1.28.1). Failures: _IBKROAuth not accepted as httpx.Auth; read_timeout_seconds was timedelta not float; Mc`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
