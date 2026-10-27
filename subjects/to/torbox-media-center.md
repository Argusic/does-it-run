# torbox-media-center

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TorBox-App/torbox-media-center, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/torbox-media-center

## Pinned environment

- Project commit: `b92b6b56d7abb6edba03b51c299cdcbedc725613`
- Test commit: `b92b6b56d7abb6edba03b51c299cdcbedc725613`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.8 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 8.8 | 2 | 2 | [run](https://argusic.com/run/a372f4e5-a305-4a96-8903-2e13c33ef1b9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install rejected: externally-managed-environment (PEP 668)`
- 5 min: `Mock API server process died between shell commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
