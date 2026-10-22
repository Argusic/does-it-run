# mcp-server-elasticsearch

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elastic/mcp-server-elasticsearch, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/mcp-server-elasticsearch

## Pinned environment

- Project commit: `9e64b842f22269eb214793e1a4885128dc4a8fd8`
- Test commit: `9e64b842f22269eb214793e1a4885128dc4a8fd8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 11.1 | 3 | 3 | [run](https://argusic.com/run/43f48344-a570-46ae-be9c-8679f2b5cc31) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `'cargo' not found: no Rust toolchain in container`
- 5 min: `Launched MCP server and mock Elasticsearch were killed ~10s after the launching exec returned (sandbox kills detached background children)`
- 2 min: `Mock ES died during tool call verification (same sandbox background-child kill), causing temporary connection-refused tool errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
