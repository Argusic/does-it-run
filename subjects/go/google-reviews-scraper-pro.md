# google-reviews-scraper-pro

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/georgekhananaev/google-reviews-scraper-pro, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/google-reviews-scraper-pro

## Pinned environment

- Project commit: `9772cd71f8e66388aff681c74b31a5bfcc814c3d`
- Test commit: `9772cd71f8e66388aff681c74b31a5bfcc814c3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 9 to 16.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 9 | 0 | 0 | [run](https://argusic.com/run/a40693ce-9360-425b-bd49-288b5ca1fea9) |
| 2 | pass with mocks | 92 | 16.2 | 16.8 | 2 | 2 | [run](https://argusic.com/run/771d856f-14ae-4f64-ac15-c5d900d1e128) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Chrome/Chromium browser not installed: 4 tests fail with 'Chrome not found! Install it first!'`
- 1 min: `PEP 668 externally-managed-environment blocks system pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
