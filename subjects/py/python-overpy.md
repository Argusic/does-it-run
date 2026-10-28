# python-overpy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DinoTools/python-overpy, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/python-overpy

## Pinned environment

- Project commit: `a8acf84e7182e2e315fd3627529b238f8688ee77`
- Test commit: `a8acf84e7182e2e315fd3627529b238f8688ee77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.3 to 1.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 1.3 | 1 | 1 | [run](https://argusic.com/run/909a4f5c-4a6c-4cd4-8ec1-b261a60bfcb6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pytest collection error in tests/test_json.py: ModuleNotFoundError: No module named 'simplejson'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
