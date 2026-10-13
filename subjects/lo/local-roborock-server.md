# local_roborock_server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Python-roborock/local_roborock_server, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/local-roborock-server

## Pinned environment

- Project commit: `af9cc4005ef8a143e6d1fa681e15ac48ca77406d`
- Test commit: `af9cc4005ef8a143e6d1fa681e15ac48ca77406d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 6.6 | 5 | 5 | [run](https://argusic.com/run/eb5ae39b-eb93-46bf-b48c-2bf02a49eafc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv and docker CLI are not installed in the container`
- 1 min: `PEP 668 externally-managed-environment blocked system-wide pip install`
- 6 min: `mosquitto binary (embedded broker) is not installed and system packages cannot be installed`
- 2 min: `First serve attempt failed: ConnectionRefusedError on 127.0.0.1:1883 because the mock broker had terminated with its parent shell`
- 1 min: `Cloudflare/ACM and protocol-auth require real third-party credentials`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
