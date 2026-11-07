# dograh

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dograh-hq/dograh, licensed BSD-2-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/dograh

## Pinned environment

- Project commit: `1e47eb54d22fdb07fb5f83189b06d2a976e4ff4c`
- Test commit: `1e47eb54d22fdb07fb5f83189b06d2a976e4ff4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 32.2 to 57 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 80 | 57 | 6 | 6 | [run](https://argusic.com/run/3965453b-77d8-4773-b8ab-2d5278245da7) |
| 2 | pass with mocks | 84 | 30 | 32.2 | 5 | 3 | [run](https://argusic.com/run/f8b7e4c0-ae50-4e9e-adae-5d3b8b7ef033) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pipecat submodule not checked out - git submodule init required`
- 3 min: `ts_validator requires Node.js >=22.6 but system has v18.19.1; .mts/.ts files need --experimental-strip-types`
- 8 min: `No PostgreSQL or Redis available in container - tests require both`
- `pgvector extension cannot be created - not compiled; server-dev package unavailable on archives for noble`
- `speechmatics SDK not available on PyPI, 5 tests fail at import time`

Attempt 2:

- 8 min: `speechmatics package not on PyPI (enterprise dependency) , patched service_factory.py to wrap import in try/except`
- 5 min: `aws_sdk_bedrock_runtime API incompatible with pipecat fork's Nova Sonic wrapper`
- 10 min: `No Docker available , stood up Postgres 16 and Redis 7 from extracted deb binaries`
- 1 min: `Python 3.12 installed, project requires >=3.13 in pyproject.toml , installed in 3.12 anyway, all tests pass`
- 3 min: `test_create_tts_service_camb fails due to test-isolation import ordering issue with pipecat.services.dograh.flux.stt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
