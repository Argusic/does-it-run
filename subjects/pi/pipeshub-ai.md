# pipeshub-ai

**Verdict: runs with mocks.** Argusic Score 68 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pipeshub-ai/pipeshub-ai, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pipeshub-ai

## Pinned environment

- Project commit: `1864d3d2a793037ccde57f21859895225eb7a540`
- Test commit: `1864d3d2a793037ccde57f21859895225eb7a540`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 3; wall time 44.7 to 65.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14.2 | 65.6 | 6 | 6 | [run](https://argusic.com/run/8a61fbb1-9599-49a6-9cca-7cfab89b5ff0) |
| 2 | fail | 20 | n/a | 44.7 | 0 | 0 | [run](https://argusic.com/run/73116157-03ab-4601-b0ff-0d4431fce2ee) |
| 3 | pass with mocks | 92 | 60 | 61.8 | 4 | 4 | [run](https://argusic.com/run/553ddd90-5b8e-49e7-8000-3fc493b238fb) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Node.js v18.19.1 incompatible with mocha@12 and sharp@0.35.4 which require Node >=20.9`
- `Python tests/unit/connectors/core/test_toolset_token_refresh.py: 9 tests fail`
- `Python tests/unit/containers/test_docling_container.py: test_logger_is_singleton fails`
- `Python tests/unit/sources/client/ hangs when run as a single directory`
- `Python tests/unit/api/ and tests/unit/services/ subdirs timeout when run together`
- `Docker not available cannot run integration tests`

Attempt 3:

- 8 min: `pytest-timeout 2.4.0 incompatible with pytest 9.x , hangs on test collection of multiple files`
- 5 min: `Node.js v18 available but project requires v22.15.0`
- 2 min: `sharp native module not compiled for platform`
- `No Docker in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
