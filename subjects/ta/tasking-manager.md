# tasking-manager

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hotosm/tasking-manager, licensed BSD-2-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/tasking-manager

## Pinned environment

- Project commit: `2b917a14ea7b0b76935c4e2d6985ab25764cd1c9`
- Test commit: `2b917a14ea7b0b76935c4e2d6985ab25764cd1c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26.1 to 26.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 60 | 26.1 | 3 | 3 | [run](https://argusic.com/run/08fd4ac3-1a34-4eec-90ac-0a78555cd9d5) |

## What was observed on a clean machine

Attempt 1:

- 60 min: `Test suite uses Flask patterns (BaseTestCase imports create_app, Flask, flask_sqlalchemy) but the backend has been migrated to FastAPI. Tests fail to import because create_app and Flask SQLAlchemy session are no longer defined in the backen`
- 10 min: `Frontend npm install hangs indefinitely , likely network connectivity issue or large dependency graph timing out.`
- 20 min: `PostgreSQL not available on system (no apt, no root). Required for both runtime and tests.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
