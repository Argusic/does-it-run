# antigravity-sdk-python

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google-antigravity/antigravity-sdk-python, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/antigravity-sdk-python

## Pinned environment

- Project commit: `12f9a4c3becf487302dc799b0f59054f01f3ddb9`
- Test commit: `12f9a4c3becf487302dc799b0f59054f01f3ddb9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 11.7 | 1 | 1 | [run](https://argusic.com/run/0839d130-e024-4250-a7cf-e14d23e42c56) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Failed tests: 10 tests crashed with RuntimeError: Could not find default localharness binary in clean checkout where binary is absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
