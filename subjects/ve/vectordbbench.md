# VectorDBBench

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zilliztech/VectorDBBench, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vectordbbench

## Pinned environment

- Project commit: `1760db148b951363f2282261f30179dfd2ce3790`
- Test commit: `1760db148b951363f2282261f30179dfd2ce3790`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 21.6 to 36.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 36.3 | 0 | 0 | [run](https://argusic.com/run/0248766f-27e5-4f5b-8c8b-ee82aad0b0ef) |
| 2 | pass | 100 | 12 | 21.6 | 6 | 6 | [run](https://argusic.com/run/12e16962-0090-445a-8fa4-f894ed68502e) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `PEP 668 externally managed environment blocks system pip install`
- 3 min: `Missing optional deps: opensearch-py, chromadb, pinecone, elasticsearch, mysql-connector-python, turbopuffer, pyvespa, flask`
- 2 min: `test_elasticsearch_cloud.py imports broken ElasticsearchConfig from wrong module`
- 1 min: `test_models.py merge test globs legacy dbPrices.json without run_id key`
- 2 min: `test_bench_runner.py uses DB.Milvus.config() and CaseType.PerformanceSZero which don't exist`
- 2 min: `test_fts_filter_runner.py mocks lack case_config attr needed by CaseRunner`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
