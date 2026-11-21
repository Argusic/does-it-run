# PyPDFForm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chinapandaman/PyPDFForm, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pypdfform

## Pinned environment

- Project commit: `3fbce223d3de4729f42df34cfe4f52c706c2de95`
- Test commit: `3fbce223d3de4729f42df34cfe4f52c706c2de95`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.7 to 52.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 52.6 | 0 | 0 | [run](https://argusic.com/run/ef29c3f8-884d-4b29-bc96-de474a9f6875) |
| 2 | pass | 100 | 2 | 9.7 | 1 | 1 | [run](https://argusic.com/run/14db0e59-da0c-4358-8ba5-8f2ec952dbd4) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `CLI assertion test_create_grid_invalid_range failed because typer/click error messages changed from 'is not in the range' to 'Input should be less than or equal to 1'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
