# VoicEra

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/COSS-India/VoicEra, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/voicera

## Pinned environment

- Project commit: `2960b281857697583e6694fa837c4138d18247d0`
- Test commit: `2960b281857697583e6694fa837c4138d18247d0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.8 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 8 | 8.1 | 4 | 4 | [run](https://argusic.com/run/3199c83b-4cf9-4c73-bab5-69e2f859ff68) |
| 2 | fail | 50 | 25 | 4.8 | 5 | 5 | [run](https://argusic.com/run/a9ce1b06-3012-42d1-aee8-2b7904c9a87c) |

## What was observed on a clean machine

Attempt 1:

- `API startup fails: FerretDB (MongoDB-compatible), MinIO, and Redis are required external services not running in container`
- `Frontend build fails: requires Node.js >=20.9.0 but container has Node.js 18.19.1 only`
- 3 min: `3 tests referencing 'bulbul:v2' failed because catalog was updated to 'bulbul:v3' only`
- `model-server/test_env_example.py: environment variables referenced in Docker Compose files missing from .env.example (docs gap, not a code bug)`

Attempt 2:

- 1 min: `Missing pytest-asyncio plugin caused 24 async test failures`
- 2 min: `Catalog updated bulbul:v2 to bulbul:v3 but 3 tests still referenced v2`
- 2 min: `test_sarvam_voice_options_split_by_model asserted anushka voice not in v3 catalog`
- `Node.js 18.19.1 too old for Next.js (needs >=20.9.0); frontend cannot build`
- `Docker not available; cannot start full application stack or run docker-dependent tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
