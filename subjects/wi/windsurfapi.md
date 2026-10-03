# WindsurfAPI

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dwgx/WindsurfAPI, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/windsurfapi

## Pinned environment

- Project commit: `a2ba9b53133236b5cb1b6540aa0414d7d400bb8f`
- Test commit: `a2ba9b53133236b5cb1b6540aa0414d7d400bb8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 7.6 to 35.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 35.6 | 4 | 4 | [run](https://argusic.com/run/5e1aea6d-3eee-4e25-b7a8-74d4b8ac8f76) |
| 2 | fail | 20 | n/a | 7.6 | 0 | 0 | [run](https://argusic.com/run/4d670e38-6d86-405d-a1e3-d1b324fb7072) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 in container , project requires >=20`
- 5 min: `test/devin-connect.test.js: deadlineMs timer with .unref() did not fire (event loop resolved) on Node 22, cascading 88 cancelled tests`
- 2 min: `test/restart.test.js: Docker detection via /.dockerenv caused 2 test failures in container`
- 1 min: `test/default-on-switch-registry.test.js: WINDSURFAPI_RESTART_SUPERVISED not in default-on LEDGER`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
