# eec

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wangguanquan/eec, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/eec

## Pinned environment

- Project commit: `08e4c50fe48b72ca312a2bb4d708fff261d87ac5`
- Test commit: `08e4c50fe48b72ca312a2bb4d708fff261d87ac5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 6.8 | 3 | 3 | [run](https://argusic.com/run/5f1199e7-4766-4f0e-97ba-d84ab4478169) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Java not installed`
- 1 min: `Maven not installed`
- 1 min: `PictureTest failed (5 failures) - no ~/Pictures directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
