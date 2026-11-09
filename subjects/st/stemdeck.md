# stemdeck

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/stemdeckapp/stemdeck, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/stemdeck

## Pinned environment

- Project commit: `96647d715fc4a7e6abbcc4875016df1595fad58f`
- Test commit: `96647d715fc4a7e6abbcc4875016df1595fad58f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.7 to 19.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 19.5 | 1 | 1 | [run](https://argusic.com/run/7f1fe170-b721-48bc-9273-e5e7b0bc270a) |
| 2 | pass | 100 | 2.5 | 11.7 | 1 | 1 | [run](https://argusic.com/run/e9007e44-6f89-4592-b223-833a624c3caa) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `diffq C extension build failed: missing Python.h (python3.12-dev headers not installed)`

Attempt 2:

- 2.5 min: `uv sync failed: Python.h not found when building diffq (C extension). Package libpython3.12-dev was not installed system-wide.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
