# winter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wintercms/winter, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/winter

## Pinned environment

- Project commit: `44e9d68f8301ef85b6d7800a43be09ff06feccfa`
- Test commit: `44e9d68f8301ef85b6d7800a43be09ff06feccfa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.3 to 22.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 22.3 | 2 | 2 | [run](https://argusic.com/run/7579d63b-04ae-458d-ba34-b375c5fc2e5b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP 8.4 was not installed in the container`
- `PHP 8.4.21 static binary segfaults during shutdown cleanup after tests pass , affects 12/48 test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
