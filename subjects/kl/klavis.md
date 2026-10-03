# klavis

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Klavis-AI/klavis, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/klavis

## Pinned environment

- Project commit: `45c9f7da83d1cf43f7429b96f9c8e8153542ea1e`
- Test commit: `45c9f7da83d1cf43f7429b96f9c8e8153542ea1e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.6 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 11 | 14.6 | 4 | 4 | [run](https://argusic.com/run/6dc26724-c9ac-4987-a299-df0a6d7494a1) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `mcp v2.2.0 renamed streamablehttp_client import to streamable_http_client`
- 3 min: `mcp v2.2.0 replaced @server.list_tools()/@server.call_tool() decorators with on_list_tools=/on_call_tool= constructor kwargs`
- 2 min: `SseServerTransport.connect_sse now sends the HTTP response internally via EventSourceResponse; handle_sse returning Response() caused double-response RuntimeError`
- 1 min: `test_sync_with_http_server assertion matched old HTTPTransport(url=...,mode=...,headers=...) signature`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
