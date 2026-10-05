# docling

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/docling-project/docling, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/docling

## Pinned environment

- Project commit: `734e8f0d69071355c0aea98bed33a7f397eba1b6`
- Test commit: `734e8f0d69071355c0aea98bed33a7f397eba1b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 74.2 to 74.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 74.2 | 4 | 4 | [run](https://argusic.com/run/91a99480-508e-41c7-a274-6382116fae35) |

## What was observed on a clean machine

Attempt 1:

- 12.5 min: `pytest-asyncio 1.4.0 strict mode hangs on module-scoped fixtures (affects e2e verification tests in test_backend_epub.py, test_backend_email.py, test_backend_docling_parse.py, etc.)`
- `test_email_backend_collapses_line_breaks_in_headers assertion failure: QP-encoded header value differs from expected plain-text value`
- `No module 'torch' , torch-dependent backends (image_native, extraction models) cannot be tested`
- 2 min: `/tmp disk full during pip install (7.8GB total)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
