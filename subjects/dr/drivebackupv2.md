# DriveBackupV2

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MaxMaeder/DriveBackupV2, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/drivebackupv2

## Pinned environment

- Project commit: `c89981401ae92435df7d0d0c105fffb33b9f6ea9`
- Test commit: `c89981401ae92435df7d0d0c105fffb33b9f6ea9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 4.6 | 3 | 3 | [run](https://argusic.com/run/32798317-e39d-48a2-b69c-2d5c877ccb3f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java runtime in container`
- 1 min: `No Maven build tool in container`
- 2 min: `Authenticator requires Firebase credentials (GOOGLE_CREDENTIALS env var) and real OAuth client secrets`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
