# antigravity-sdk-python

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google-antigravity/antigravity-sdk-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/antigravity-sdk-python

## Pinned environment

- Project commit: `12f9a4c3becf487302dc799b0f59054f01f3ddb9`
- Test commit: `12f9a4c3becf487302dc799b0f59054f01f3ddb9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 6.6 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 11.7 | 1 | 1 | [run](https://argusic.com/run/0839d130-e024-4250-a7cf-e14d23e42c56) |
| 2 | pass with mocks | 92 | 14 | 6.6 | 2 | 2 | [run](https://argusic.com/run/15b6f9c3-c4b5-4c49-831d-f72e23f8493e) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Failed tests: 10 tests crashed with RuntimeError: Could not find default localharness binary in clean checkout where binary is absent`

Attempt 2:

- 3 min: `Missing protobuf compiled modules (*_pb2.py) in google/antigravity/proto/`
- 4 min: `Test RuntimeError: Could not find default localharness binary in several test classes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
