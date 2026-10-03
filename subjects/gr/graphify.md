# graphify

**Verdict: runs.** Argusic Score 66.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Graphify-Labs/graphify, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/graphify

## Pinned environment

- Project commit: `33362d969292b57eda82f3fbd9eb5f3f5bc9bbc2`
- Test commit: `33362d969292b57eda82f3fbd9eb5f3f5bc9bbc2`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 0.4 to 35.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 35.8 | 1 | 1 | [run](https://argusic.com/run/3d009041-3769-4a46-9eaf-4f29104fa9dc) |
| 2 | pass | 80 | 0.5 | 11.3 | 1 | 0 | [run](https://argusic.com/run/7d8e0538-83b6-472a-a537-d34186082a7d) |
| 3 | fail | 20 | n/a | 0.4 | 0 | 0 | [run](https://argusic.com/run/726a1483-2f64-4eb7-8c70-cb9b95067af6) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `tree-sitter-dm build failure: missing Python.h (python3.12-dev headers not installed in container)`

Attempt 2:

- `test_skillgen.py: 11 tests fail because the repo is a shallow clone with only 1 commit; tests reference specific SHAs not in history (47042be, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
