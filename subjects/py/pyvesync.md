# pyvesync

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/webdjoe/pyvesync, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pyvesync

## Pinned environment

- Project commit: `58eee3bdbfbaac98d64cd0dd4fd66e1f1c24ab8e`
- Test commit: `58eee3bdbfbaac98d64cd0dd4fd66e1f1c24ab8e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 8.4 | 5 | 5 | [run](https://argusic.com/run/5ad66907-ec53-4e7e-b322-015ce7e4f24f) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Mock server process was SIGHUP-killed when launched with '&' in the non-interactive shell (connection refused on 127.0.0.1:8931), an environment/harness artifact, not a repo bug`
- 6 min: `My first API mock compared the plain-text password while the library sends MD5(password) (RequestGetTokenModel.hash_password), so login failed with the library's real VeSyncLoginError - mock-schema mismatch`
- 5 min: `My device-list fixture lacked the required 'type' field, so mashumaro raised MissingField('type') in ResponseDeviceDetailsModel - mock-schema mismatch`
- 4 min: `My device-status endpoint path was wrong for the ESW15-USA outlet (library posts to /cloud/v1/deviceManaged/deviceStatus) - mock-schema mismatch`
- 2 min: `My harness script used dev.state.device_status and indexing, but the library exposes state status via dev.state.device_status/is_on and DeviceContainer is a set - harness-script mistakes I fixed via next(iter(...))`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
