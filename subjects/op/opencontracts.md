# OpenContracts

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Open-Source-Legal/OpenContracts, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/opencontracts

## Pinned environment

- Project commit: `1e859dcea0f083f374c160a04244f93bca5b989c`
- Test commit: `1e859dcea0f083f374c160a04244f93bca5b989c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 55.6 to 77.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 77.3 | 3 | 3 | [run](https://argusic.com/run/ffe8e6fc-c8fc-4a77-949a-b9681eb03281) |
| 2 | pass with mocks | 92 | 5 | 55.6 | 5 | 5 | [run](https://argusic.com/run/12d99f02-4441-42ed-9e34-eb51e52a8055) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_analyzers::test_analyzerz fails with Not all requests have been executed - needs Celery worker at localhost:8000 (Docker microservice)`
- `pdfredact module missing - opencontractserver.pipeline.post_processors.pdf_redactor failed to import`
- `test_multimodal_integration.py and test_pdf_outline_enricher.py cannot be collected without DATABASE_URL set (pytest-django collects all test files at startup)`

Attempt 2:

- 5 min: `config/settings/test.py sets PostgreSQL-specific connection options unconditionally, crashing on SQLite`
- 25 min: `No PostgreSQL or pgvector available in container`
- 5 min: `Django migrations with CREATE INDEX CONCURRENTLY cause hangs`
- 1 min: `Missing reportlab package in test fixture`
- 5 min: `Test DB needs pgvector and pg_trgm pre-installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
