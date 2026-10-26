# knowledge-rag

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lyonzin/knowledge-rag, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/knowledge-rag

## Pinned environment

- Project commit: `d3715d7ac2248657bc55430d93daba16fa82e375`
- Test commit: `d3715d7ac2248657bc55430d93daba16fa82e375`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.9 | 2 | 2 | [run](https://argusic.com/run/3f71b019-8d59-4d72-8651-af3e4250565d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `system Python externally-managed-environment (PEP 668) prevented direct pip install`
- `onnxruntime pthread_setaffinity_np failed for thread , EINVAL during CPU core affinity (cosmetic)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
