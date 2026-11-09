# mcpo

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-webui/mcpo, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcpo

## Pinned environment

- Project commit: `788ff92e5288a899a743a252edd5748f4ad4ab1f`
- Test commit: `788ff92e5288a899a743a252edd5748f4ad4ab1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.7 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.8 | 2 | 2 | [run](https://argusic.com/run/c224c4a4-d053-48c0-9bff-006f284de03f) |
| 2 | pass with mocks | 92 | 3 | 2.7 | 1 | 1 | [run](https://argusic.com/run/06a21af5-88b4-478c-afff-4d822e9603ac) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install -e .[dev] did not include pytest and pytest-asyncio`
- 1 min: `mcp v2.2.0 installed despite pyproject.toml requiring >=1.17.0; mcp v2 renamed McpError->MCPError and streamablehttp_client->streamable_http_client, breaking imports`

Attempt 2:

- 1 min: `pip install failed: PEP 668 externally-managed environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
