# mobilerun

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/droidrun/mobilerun, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mobilerun

## Pinned environment

- Project commit: `4f168cbbfa3134a7acca6ab7f96d8d059c249df5`
- Test commit: `4f168cbbfa3134a7acca6ab7f96d8d059c249df5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23.89 | 5.1 | 1 | 1 | [run](https://argusic.com/run/1dd1f181-825c-4da0-ab40-a2416ccb1f42) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Missing optional dependency 'langfuse' , 12 test_langfuse_v4.py tests failed with ModuleNotFoundError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
