# crawlee-python

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apify/crawlee-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/crawlee-python

## Pinned environment

- Project commit: `45bb0e25df8fdad3caf0e756e32c2063717da4ce`
- Test commit: `45bb0e25df8fdad3caf0e756e32c2063717da4ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.5 | 7.5 | 2 | 2 | [run](https://argusic.com/run/200f39e3-56d7-43b1-826d-c1e470ed4df5) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `uv binary not in PATH after pip install to user site`
- 0.5 min: `Playwright Firefox browser not installed (only chromium was installed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
