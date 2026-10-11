# minima

**Verdict: runs with mocks.** Argusic Score 87 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Minima-AI-Inc/minima, licensed MPL-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/minima

## Pinned environment

- Project commit: `e6cc03f38be4c1019987aeb9ef8b6cf3ab5634a5`
- Test commit: `e6cc03f38be4c1019987aeb9ef8b6cf3ab5634a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 36.8 to 36.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 37 | 36.8 | 8 | 6 | [run](https://argusic.com/run/cf99fbf0-fc95-4392-91b6-e22d8fa2fecf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Electron SUID sandbox not configured correctly - needs --no-sandbox flag`
- 2 min: `Chat test failed: scrollIntoView not in jsdom`
- 1 min: `Chat test failed: placeholder text mismatch`
- 3 min: `sentence-transformers import fails: numpy/scipy version conflict`
- 3 min: `LangChain version conflicts between packages`
- 5 min: `Indexer search via API returns empty with in-memory Qdrant`
- 1 min: `Docker not available - Qdrant, Ollama containers cannot run`
- 1 min: `Firebase credentials required for linker service`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
