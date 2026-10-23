# vector-db-benchmark

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qdrant/vector-db-benchmark, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vector-db-benchmark

## Pinned environment

- Project commit: `871a0b2ea6d67045f3d72958a158ef7596353c74`
- Test commit: `871a0b2ea6d67045f3d72958a158ef7596353c74`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.7 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 2.7 | 3 | 3 | [run](https://argusic.com/run/40e984bc-ac00-444f-beef-a166c285a091) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Test failed: test_parse_converts_exact_match expected double-quoted syntax but parser produces curly-braces syntax`
- 1 min: `pytest fails importing 'engine' module when run without -m flag (package-mode=false skips installing package into site-packages)`
- 1 min: `First poetry install failed due to missing virtualenv cshell deactivate file (race condition in virtualenv), resolved by re-running`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
