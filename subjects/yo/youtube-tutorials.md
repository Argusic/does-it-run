# youtube-tutorials

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/owainlewis/youtube-tutorials, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/youtube-tutorials

## Pinned environment

- Project commit: `5b3d3c9a136dc797c0da1427406c9a53fefbee5c`
- Test commit: `5b3d3c9a136dc797c0da1427406c9a53fefbee5c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 6.6 | 4 | 4 | [run](https://argusic.com/run/6671cb3a-8638-4c0d-b9ae-c6e60c3eb887) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `just command not found (Python 'just' package is wrong; need casey/just binary)`
- 1 min: `python-dateutil missing (dependency of Python 'just' package)`
- 1 min: `terraform not found (needed for audit-terraform and deploy-ai-on-gcp tests)`
- 1 min: `go not found (needed for micro-neo tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
