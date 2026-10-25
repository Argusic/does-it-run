# VeritasGraph

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bibinprathap/VeritasGraph, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/veritasgraph

## Pinned environment

- Project commit: `37e86dd2aa0c3851eeb2393593621b8cd2a8a38f`
- Test commit: `37e86dd2aa0c3851eeb2393593621b8cd2a8a38f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.9 to 15.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 15.9 | 4 | 4 | [run](https://argusic.com/run/6b7d44b8-ad3b-466c-9b80-259acc0e7336) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `test_pipeline_invokes_loopback_tool_and_traces_results failed: orchestrator now skips LLM-backed graph answer tools (Graph Retriever -> /graphrag/query), preventing the tool from being invoked`
- 10 min: `test_pipeline_blocks_external_tools_by_default failed: Web Search tool is 'disabled' in seed data and auto-added MCP loopback tools are invoked instead`
- 5 min: `veritas-reason tests/kg/ needed scipy, gensim (missing from venv)`
- 5 min: `veritas-reason tests/parse/ needed python-docx, GitPython, openpyxl, matplotlib, scikit-learn, plotly`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
