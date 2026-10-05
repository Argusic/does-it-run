# mcp-memory-service

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/doobidoo/mcp-memory-service, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-memory-service

## Pinned environment

- Project commit: `4a225345976076a68655692d52c09b177666758e`
- Test commit: `4a225345976076a68655692d52c09b177666758e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.9 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 19.9 | 2 | 2 | [run](https://argusic.com/run/ccee5182-9475-42fd-9555-9dae6f5606e1) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test_stop_refuses_to_kill_foreign_listener_without_force failed: '_find_process_on_port' uses 'lsof' which is not installed in this container, so it returns None and the foreign listener is never detected`
- `test_retrieve_exact_query_finds_something (benchmark) fails: hash-embedding fallback mode cannot perform accurate semantic search without ONNX/transformers dependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
