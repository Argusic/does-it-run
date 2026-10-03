# code-graph-rag

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vitali87/code-graph-rag, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/code-graph-rag

## Pinned environment

- Project commit: `511d6f6aecdcb55bef1a639220eee70780bfbf4b`
- Test commit: `511d6f6aecdcb55bef1a639220eee70780bfbf4b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 55.5 to 55.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 52 | 55.5 | 3 | 1 | [run](https://argusic.com/run/d9610942-f0ae-4843-b4fe-62aa7a2940b1) |

## What was observed on a clean machine

Attempt 1:

- `python3-dev not installed; tree-sitter-c/C++ grammars fail to build from source (Python.h missing)`
- 5 min: `pytest-asyncio 1.3.0 incompatible with pytest 9.x (asyncio_mode config unknown)`
- `Docker not available; Memgraph/Qdrant stack cannot start`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
