# librespot-python

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kokarare1212/librespot-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/librespot-python

## Pinned environment

- Project commit: `683d9e76f91ba7ae03919494dac8d899ca505651`
- Test commit: `683d9e76f91ba7ae03919494dac8d899ca505651`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 7.1 to 14.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 24 | 7.1 | 0 | 0 | [run](https://argusic.com/run/e377a165-0263-4b54-8595-6e2882cdf4de) |
| 2 | fail | 80 | 0.5 | 14.5 | 2 | 2 | [run](https://argusic.com/run/e62a2e0f-59e5-448d-91e7-360c180592c8) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `ZeroconfServer failed to start/close due to zeroconf 0.151.3 API change: start() called after register_service() and close() asserted loop is not None because start() was never called on the main thread. Also HttpRunner.close() was a no-op,`
- 3 min: `Session.Builder.stored() raised UnicodeDecodeError when parsing base64-encoded JSON stored credentials because it tried base64 decode first without catching UnicodeDecodeError.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
