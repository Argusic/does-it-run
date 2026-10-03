# pinchtab

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pinchtab/pinchtab, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/pinchtab

## Pinned environment

- Project commit: `83666d2271002fb81f7ee69862ec12aa29facfd8`
- Test commit: `83666d2271002fb81f7ee69862ec12aa29facfd8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 40.8 to 40.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 42 | 40.8 | 3 | 3 | [run](https://argusic.com/run/e2a5ffd2-8f75-4e46-8385-061d93662b7f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed in container`
- 8 min: `No Chrome/Chromium browser found in container`
- 3 min: `Test failure: internal/activity/TestQuerySourcesNarrowsFileWalkAndSkipsUnrequestedSource , hardcoded date 2026-09-12 fell outside 7-day retention window, so Query() pruned the test files before reading them`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
