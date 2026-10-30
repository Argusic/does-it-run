# OpenGateLLM

**Verdict: runs with mocks.** Argusic Score 89.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/etalab-ia/OpenGateLLM, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/opengatellm

## Pinned environment

- Project commit: `4faf1f3b119cf0cc112ebc615203cf122b4a91dd`
- Test commit: `4faf1f3b119cf0cc112ebc615203cf122b4a91dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30.2 to 30.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 89.14 | 12 | 30.2 | 7 | 6 | [run](https://argusic.com/run/c0b96fda-9b38-4e6e-91d0-83575f33f4a3) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `alembic downgrade base failed: type "collectionvisibility" already exists (enum type never dropped with its table)`
- 14 min: `alembic downgrade failed: Cannot emit DROP CONSTRAINT ... has no name in revisions 4cbcc969c660, 9fd5b6491d48, 9ba1f6a21f20, 2d2550e0771d, c1e54102255e, 8c5ae2a3d4d0, e78eaed1bcb2`
- 4 min: `revision 9ba1f6a21f20 downgrade failed: NotNullViolation adding NOT NULL columns to tables with rows`
- 5 min: `revision 9ba1f6a21f20 downgrade failed: relation "model" does not exist (model_client created before model)`
- 5 min: `full downgrade leaves httpmethod/limittype/permissiontype enum types behind, so a later upgrade fails with duplicate type`
- 12 min: `upgrade head after a full downgrade base still fails: type "modeltype" already exists`
- 8 min: `docker/Postgres/Redis absent in container; background processes spawned by exec_command were reaped after the call (mock provider and a Redis helper died)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
