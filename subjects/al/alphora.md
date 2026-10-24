# alphora

**Verdict: runs with mocks.** Argusic Score 52.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/opencmit/alphora, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/alphora

## Pinned environment

- Project commit: `3885e73b8d610287ed0a04f5c94b4134ef10933e`
- Test commit: `3885e73b8d610287ed0a04f5c94b4134ef10933e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 2.2 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 2.2 | 0 | 0 | [run](https://argusic.com/run/ca9dd725-1877-4378-9d96-a021b33308b9) |
| 2 | pass with mocks | 85.33 | 3 | 16.6 | 3 | 2 | [run](https://argusic.com/run/9bf7323c-688d-4f70-bca6-4d8ab5372d05) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `memory/manager.py inject() failed on plain string -> AttributeError: 'str' object has no attribute 'to_dict'`
- 1 min: `sync long_response path sent unexpected prompt_id to LongResponseGenerator`
- `Docker sandbox unavailable (no Docker socket)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
