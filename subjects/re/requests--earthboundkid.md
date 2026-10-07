# requests

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/earthboundkid/requests, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/8c34c7d7-c931-473b-9997-3b11b6a7617c

## Pinned environment

- Project commit: `e5187a4ef8a22592cb50916308078c49faf4ace5`
- Test commit: `e5187a4ef8a22592cb50916308078c49faf4ace5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 8.4 | 1 | 1 | [run](https://argusic.com/run/8c34c7d7-c931-473b-9997-3b11b6a7617c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go (golang.org) compiler not pre-installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
