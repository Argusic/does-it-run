# OpenManus

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FoundationAgents/OpenManus, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openmanus

## Pinned environment

- Project commit: `3309bf4e416fb1c74b008f3e86494439a31bad53`
- Test commit: `3309bf4e416fb1c74b008f3e86494439a31bad53`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.8 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.5 | 1 | 1 | [run](https://argusic.com/run/6563590c-4e96-4c95-9356-4478101ddb39) |
| 2 | pass | 90 | 3 | 5.8 | 2 | 1 | [run](https://argusic.com/run/b48ea45b-00c2-456b-bd4f-83fc278c3ae3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `DaytonaSettings.daytona_api_key had no default, causing ValidationError when [daytona] section missing`

Attempt 2:

- 0.5 min: `config.toml requires daytona_api_key field which is missing from config.example.toml`
- `Sandbox tests require Docker daemon, not available in this container (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
