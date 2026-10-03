# DemoGPT

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/melih-unsal/DemoGPT, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/demogpt

## Pinned environment

- Project commit: `aca748b7134549d6fa80c5c3a989779919697095`
- Test commit: `aca748b7134549d6fa80c5c3a989779919697095`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 32.7 to 54.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 32.7 | 5 | 5 | [run](https://argusic.com/run/74cf14ca-8311-490f-9d1e-f7e9b207ef6a) |
| 2 | pass with mocks | 92 | 5 | 54.7 | 7 | 7 | [run](https://argusic.com/run/f36776f9-ddc0-4b87-8a9a-f70fce362ff0) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install . failed: externally-managed Python environment`
- 2 min: `Tests failed: OPENAI_API_KEY not set`
- 1.5 min: `RAG tests failed: sentence-transformers not installed (missing dependency in pyproject.toml)`
- 0.5 min: `RAG tests failed: BaseRAG has no 'query' method (tests call rag.query but only rag.run exists)`
- 0.5 min: `RAG tests failed: ChromaDB readonly DB error when tests share same persistent_path in-process`

Attempt 2:

- 1 min: `Externally-managed Python environment prevented system-wide pip install`
- 0.5 min: `pytest not installed`
- 2 min: `Tests require OPENAI_API_KEY`
- 0.5 min: `BaseRAG has no query() method, tests call query()`
- 0.5 min: `ChromaDB 'attempt to write a readonly database' between test methods sharing persistent_path`
- 0.5 min: `Mock server returned static 'Ankara' answer regardless of RAG context, failing assertions for '40' or '28'`
- 12 min: `sentence-transformers package not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
