# crewAI

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crewAIInc/crewAI, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/crewai

## Pinned environment

- Project commit: `dd4a1062913375cfb4782ba0936a32d9ebbfcb3d`
- Test commit: `dd4a1062913375cfb4782ba0936a32d9ebbfcb3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 19.1 to 59 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 19.1 | 0 | 0 | [run](https://argusic.com/run/8c797de3-dc77-47c5-bc09-e6e2b2dbdd07) |
| 2 | pass | 100 | 15 | 59 | 5 | 5 | [run](https://argusic.com/run/37d80ecd-1722-4cad-9287-2ae7e6b430ea) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `uv not installed in environment`
- 1 min: `a2a-sdk not installed (ModuleNotFoundError: a2a)`
- 1 min: `qdrant-client not installed (ModuleNotFoundError: qdrant_client)`
- 3 min: `boto3, google-genai, azure SDKs not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
