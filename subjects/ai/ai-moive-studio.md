# ai-moive-studio

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/869413421/ai-moive-studio, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-moive-studio

## Pinned environment

- Project commit: `4e0810eab1d84ed1424883b88f6b4cd232b74724`
- Test commit: `4e0810eab1d84ed1424883b88f6b4cd232b74724`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.9 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.8 | 21.9 | 5 | 5 | [run](https://argusic.com/run/3b920d5a-07fe-4be4-b8bd-ac56965ab347) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing system library libmagic (python-magic dependency)`
- 2 min: `Missing FileProcessingStatus and SupportedFileType enums referenced by tests`
- 5 min: `Stale test imports: src.api.upload, src.api.files, src.api.projects, src.core.auth0_auth`
- 0.5 min: `Stale test import: src.tasks.task (module is src.tasks.project)`
- `No PostgreSQL/Redis/MinIO (no Docker) - API register fails`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
