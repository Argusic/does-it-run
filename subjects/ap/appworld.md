# appworld

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/StonyBrookNLP/appworld, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/appworld

## Pinned environment

- Project commit: `42b5bcf3cd334fee33f0c37c02070a9f5807add5`
- Test commit: `42b5bcf3cd334fee33f0c37c02070a9f5807add5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.4 to 37.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 37.4 | 5 | 5 | [run](https://argusic.com/run/d0f68967-d8cb-4435-986b-44cf3338df1c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `PEP 668 externally-managed-environment blocked system pip install`
- 1 min: `fastapi 0.146.0 / pydantic 2.14.1 incompatibility: match_type() takes 2 positional arguments but 3 were given`
- 3 min: `Bundle files (.bundle) were Git LFS pointers (193 bytes) not actual content`
- 2 min: `OrderItem model datetimes used SQLModel default UTCDateTime requiring tz-aware values, but AppWorld uses naive PendulumDateTimes`
- 1 min: `Missing openapi_spec_validator package for test_prepare_api_docs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
