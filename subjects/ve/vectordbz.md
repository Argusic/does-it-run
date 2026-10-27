# vectordbz

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vectordbz/vectordbz, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vectordbz

## Pinned environment

- Project commit: `57d51d2549ba01e8b0e4a641f3a8772c8697e59f`
- Test commit: `57d51d2549ba01e8b0e4a641f3a8772c8697e59f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30.4 to 30.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 29 | 30.4 | 5 | 5 | [run](https://argusic.com/run/1e75a75d-9500-452c-9302-c1dd86f5793e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js version mismatch - system has v18.19.1, project requires >=22.12.0`
- 2 min: `Corrupted Vite build artifacts from prior failed package attempt caused Electron SyntaxError: Unexpected end of input`
- 1 min: `Electron main.js entry-point had duplicated content after rebuild`
- `All 8 database integration test files fail - require Docker containers for Qdrant, Weaviate, ChromaDB, Milvus, pgvector, Pinecone, Elasticsearch, RedisSearch (docker not available in container)`
- `npm run package (electron-forge make) runs out of memory (OOM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
