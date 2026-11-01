# docling

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/docling-project/docling, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/docling

## Pinned environment

- Project commit: `734e8f0d69071355c0aea98bed33a7f397eba1b6`
- Test commit: `734e8f0d69071355c0aea98bed33a7f397eba1b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 22.3 to 74.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 74.2 | 4 | 4 | [run](https://argusic.com/run/91a99480-508e-41c7-a274-6382116fae35) |
| 2 | pass | 93.33 | 15 | 22.3 | 3 | 2 | [run](https://argusic.com/run/96700cd6-e508-4e9f-b79f-f8621cd2b6a7) |

## What was observed on a clean machine

Attempt 1:

- 12.5 min: `pytest-asyncio 1.4.0 strict mode hangs on module-scoped fixtures (affects e2e verification tests in test_backend_epub.py, test_backend_email.py, test_backend_docling_parse.py, etc.)`
- `test_email_backend_collapses_line_breaks_in_headers assertion failure: QP-encoded header value differs from expected plain-text value`
- `No module 'torch' , torch-dependent backends (image_native, extraction models) cannot be tested`
- 2 min: `/tmp disk full during pip install (7.8GB total)`

Attempt 2:

- 12 min: `make setup failed: webrtcvad==2.0.10 (via resemblyzer, docling-slim[format-video]) could not build: fatal error Python.h and then x86_64-linux-gnu/python3.12/pyconfig.h missing (container has no python3-dev headers, no root for apt)`
- 1 min: `pip install uv rejected by PEP 668 externally-managed-environment`
- 25 min: `2 core-lane tests fail deterministically on CPU: test_extraction_with_pydantic_instance_template and test_extraction_with_pydantic_class_template assert extracted total 3667.35 == 3949.75; root cause is polyfactory serializing the pydantic`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
