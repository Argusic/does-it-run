# lamda

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/firerpa/lamda, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/lamda

## Pinned environment

- Project commit: `fd675997269fc9e6e9e5c52aee6a35db065ce7b6`
- Test commit: `fd675997269fc9e6e9e5c52aee6a35db065ce7b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5.2 | 6.8 | 1 | 1 | [run](https://argusic.com/run/4248b81b-6f1e-4cce-8508-b432c0873a27) |

## What was observed on a clean machine

Attempt 1:

- 2.1 min: `System Python 3 is externally managed (PEP 668), preventing direct pip install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
