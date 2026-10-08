# OpenContracts

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Open-Source-Legal/OpenContracts, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/opencontracts

## Pinned environment

- Project commit: `1e859dcea0f083f374c160a04244f93bca5b989c`
- Test commit: `1e859dcea0f083f374c160a04244f93bca5b989c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 77.3 to 77.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 77.3 | 3 | 3 | [run](https://argusic.com/run/ffe8e6fc-c8fc-4a77-949a-b9681eb03281) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_analyzers::test_analyzerz fails with Not all requests have been executed - needs Celery worker at localhost:8000 (Docker microservice)`
- `pdfredact module missing - opencontractserver.pipeline.post_processors.pdf_redactor failed to import`
- `test_multimodal_integration.py and test_pdf_outline_enricher.py cannot be collected without DATABASE_URL set (pytest-django collects all test files at startup)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
