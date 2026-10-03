# artemis

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/artemis, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/artemis

## Pinned environment

- Project commit: `371aa6df56880643da57b30da936e9812fb0ec66`
- Test commit: `371aa6df56880643da57b30da936e9812fb0ec66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26.4 to 26.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 26.4 | 3 | 3 | [run](https://argusic.com/run/90a7909c-c473-4392-b3c0-a4bff4a1a833) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `adb_server_manifest fixture descriptions mismatch MCP v1.29.0 indentation`
- 3 min: `subprocess.CREATE_NEW_PROCESS_GROUP does not exist on Linux in device_utils test`
- 3 min: `video frame count assertion 43-47 fails; actual frames 77`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
