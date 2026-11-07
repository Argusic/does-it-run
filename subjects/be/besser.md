# BESSER

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BESSER-PEARL/BESSER, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/besser

## Pinned environment

- Project commit: `7aefb2329f25484ccf1aee507dc04b231fc32081`
- Test commit: `7aefb2329f25484ccf1aee507dc04b231fc32081`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 23 | 1 | 1 | [run](https://argusic.com/run/c3f8a532-9b0b-4acb-a14f-79a909057562) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `bubblewrap (bwrap) not installed - shell sandbox unavailable, causing 2 test failures in test_derived_enum_entity_can_be_created.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
