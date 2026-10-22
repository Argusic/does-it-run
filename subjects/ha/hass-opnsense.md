# hass-opnsense

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/travisghansen/hass-opnsense, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/hass-opnsense

## Pinned environment

- Project commit: `d76f09bf7d23444d795a8be17b2bc8ec84e328af`
- Test commit: `d76f09bf7d23444d795a8be17b2bc8ec84e328af`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 2.8 | 1 | 1 | [run](https://argusic.com/run/fd708797-5cb5-4da8-92a7-5bd28ac23ef9) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `System Python is 3.12.3 but project requires >=3.14.2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
