# google-search-results-python

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/serpapi/google-search-results-python, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/google-search-results-python

## Pinned environment

- Project commit: `345d31a928ff887c75f340aa7c6d33bd0d9976d2`
- Test commit: `345d31a928ff887c75f340aa7c6d33bd0d9976d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.3 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.3 | 0 | 0 | [run](https://argusic.com/run/94ed6cba-d9b6-4d72-8588-8643dfd86252) |
| 2 | pass with mocks | 92 | 4 | 11.5 | 1 | 1 | [run](https://argusic.com/run/a256683e-42c9-474f-8924-dad9153cbd89) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Existing test test_missing_ fails against real backend (returns 'Invalid API key' instead of expected 'Missing query 'q'' when using demo key and no query)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
