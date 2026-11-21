# dstask

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/naggie/dstask, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/dstask

## Pinned environment

- Project commit: `cdfd902d8439ba750d4425dc403e1f74b7e7c024`
- Test commit: `cdfd902d8439ba750d4425dc403e1f74b7e7c024`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 3.8 | 0 | 0 | [run](https://argusic.com/run/7a8d92b8-c05b-461c-931f-4a8ee41622dd) |
| 2 | pass | 100 | 4.5 | 1.8 | 1 | 1 | [run](https://argusic.com/run/f074c53b-d85b-48bf-86d5-59d755833353) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Integration tests failed because git user identity was not configured. Git commit would fail with 'Author identity unknown'. This affected 50+ integration tests.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
