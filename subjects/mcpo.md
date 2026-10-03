# mcpo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-webui/mcpo, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcpo

## Pinned environment

- Project commit: `788ff92e5288a899a743a252edd5748f4ad4ab1f`
- Test commit: `788ff92e5288a899a743a252edd5748f4ad4ab1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.8 | 2 | 2 | [run](https://argusic.com/run/c224c4a4-d053-48c0-9bff-006f284de03f) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install -e .[dev] did not include pytest and pytest-asyncio`
- 1 min: `mcp v2.2.0 installed despite pyproject.toml requiring >=1.17.0; mcp v2 renamed McpError->MCPError and streamablehttp_client->streamable_http_client, breaking imports`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
