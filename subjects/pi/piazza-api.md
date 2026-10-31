# piazza-api

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hfaran/piazza-api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/piazza-api

## Pinned environment

- Project commit: `39681fe60324c2f637c1615332db2e60818f93a2`
- Test commit: `39681fe60324c2f637c1615332db2e60818f93a2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.7 to 25.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 25.7 | 3 | 3 | [run](https://argusic.com/run/0f8c38d2-e6c3-456c-808f-e75815a7b635) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `No tests or CLI in repo; the only way to exercise is via the library calls`
- 3 min: `Mock HTTP keep-alive acted unstably through the container proxy`
- `Piazza() without login raises AttributeError instead of NotAuthenticatedError (library quirk)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
