# pyJianYingDraft

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GuanYixuan/pyJianYingDraft, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/pyjianyingdraft

## Pinned environment

- Project commit: `c3318066d964744e2bfc66f75c71745fe8cea52a`
- Test commit: `c3318066d964744e2bfc66f75c71745fe8cea52a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.4 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1 | 6.4 | 1 | 1 | [run](https://argusic.com/run/6b7b2d1a-87b6-4b7e-aaab-9df3682b1979) |
| 2 | pass with mocks | 92 | 0.3 | 6.9 | 1 | 1 | [run](https://argusic.com/run/d2e1b24b-5840-46e7-b9be-623b89f51d7e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Test test_duplicate_as_template_reuses_fallback_loader used Windows-specific backslash path separator in assertion string, which fails on Linux`

Attempt 2:

- 0.1 min: `test_duplicate_as_template_reuses_fallback_loader failed on Linux due to hardcoded Windows path separator (backslash)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
