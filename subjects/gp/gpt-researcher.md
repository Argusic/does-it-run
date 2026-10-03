# gpt-researcher

**Verdict: runs with mocks.** Argusic Score 89.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/assafelovic/gpt-researcher, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/gpt-researcher

## Pinned environment

- Project commit: `6f998577d547b1e54ec662dac63583aa11e3b84b`
- Test commit: `6f998577d547b1e54ec662dac63583aa11e3b84b`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 23.2 to 67.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 12 | 38 | 3 | 2 | [run](https://argusic.com/run/b89d9cd6-5bb7-4bc0-a7c5-7b80299d44f6) |
| 2 | pass with mocks | 92 | 9 | 67.9 | 2 | 2 | [run](https://argusic.com/run/b2a8dad6-7c79-4d3e-b001-c8ab140573fb) |
| 3 | pass with mocks | 92 | 1.7 | 23.2 | 0 | 0 | [run](https://argusic.com/run/430382d8-ca1e-4be2-9ebd-47fd35bac40b) |

## What was observed on a clean machine

Attempt 1:

- 11 min: `No pip/venv in environment , used --user --break-system-packages to install dependencies`
- 7 min: `12 of 14 test failures in full suite are import-isolation issues (package interference when all 400+ tests run together). Tests pass in isolation.`

Attempt 2:

- 10 min: `14 test files (duckduckgo_normalize, groundroute_malformed, openalex_malformed, arxiv_null_fields, vector_store_doc_guards, bs_session_none, web_base_loader_docs_guard, web_base_loader_enrichment_guard) inject fake modules into sys.modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
