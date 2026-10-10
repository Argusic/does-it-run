# OpenFic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/syrizelink/OpenFic, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/openfic

## Pinned environment

- Project commit: `8fd5078e443b0d779ea02c16b87a6fd095844c53`
- Test commit: `8fd5078e443b0d779ea02c16b87a6fd095844c53`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 11 | 3 | 3 | [run](https://argusic.com/run/93519279-259e-464d-a9d3-95dcb47dd1ee) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System pip refused with 'externally-managed-environment' (PEP 668)`
- 2 min: `8 test files failed to collect: ModuleNotFoundError: No module named 'respx'`
- 1 min: `test_create_chat_model_adds_opencode_headers_for_openai_compatible_endpoint failed: asserted 'OpenFic/0.11.1' but app_version is '0.12.0'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
