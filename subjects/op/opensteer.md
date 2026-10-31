# opensteer

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/steerlabs/opensteer, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opensteer

## Pinned environment

- Project commit: `e8ebf8c3ce009befd01bcadcc2a8b2b649f03099`
- Test commit: `e8ebf8c3ce009befd01bcadcc2a8b2b649f03099`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 1.4 to 1.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 1.4 | 4 | 4 | [run](https://argusic.com/run/90b5091a-8e81-4b7c-ac9d-7e9653d69806) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not found on PATH`
- 0.5 min: `No module named 'pytest'`
- 0.5 min: `No module named 'PIL' when collecting test_helpers.py`
- 0.5 min: `No module named 'cdp_use' when collecting test_remote.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
