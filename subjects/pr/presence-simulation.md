# presence_simulation

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/slashback100/presence_simulation, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/presence-simulation

## Pinned environment

- Project commit: `140b666cb280d01ca973e873dc964b275a91ea03`
- Test commit: `140b666cb280d01ca973e873dc964b275a91ea03`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 9.4 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 9.4 | 0 | 0 | [run](https://argusic.com/run/d8666460-489a-4572-8025-946d4e76637f) |
| 2 | pass | 100 | 10 | 10.4 | 3 | 3 | [run](https://argusic.com/run/3bca3265-ac7f-4f30-9345-54bbfa15fbf0) |

## What was observed on a clean machine

Attempt 2:

- 6 min: `pip install homeassistant failed: externally-managed-environment`
- 1 min: `pytest-homeassistant-custom-component fixture enable_custom_integrations incompatible with pytest-asyncio 0.24 (sync fixture consuming async generator)`
- 2 min: `Multiple test compatibility issues: ServiceRegistry.async_call is read-only C attr; FlowResultType is now an Enum; recorder DB setup fails in test env`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
