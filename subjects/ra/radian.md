# radian

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/randy3k/radian, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/radian

## Pinned environment

- Project commit: `545f504f672d9d02ae5603c4c42e61200117d69a`
- Test commit: `545f504f672d9d02ae5603c4c42e61200117d69a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 29.5 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/dd3014f5-f748-4dfa-970e-c4fa84d588d8) |
| 2 | pass with mocks | 92 | 28 | 29.5 | 5 | 5 | [run](https://argusic.com/run/4e59d8a0-22a1-4bca-ac6a-b1b4f6f005ce) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `No R binary or shared library available in container`
- 2 min: `R binary fails to load due to missing libtirpc.so.3`
- 3 min: `R default packages (utils, stats) fail to load with invalid editor error`
- 5 min: `rchitect exec_host re-exec loses LD_LIBRARY_PATH entries for extracted R installation`
- 10 min: `CRAN packages (askpass, renv, reticulate) required by 7 tests cannot be installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
