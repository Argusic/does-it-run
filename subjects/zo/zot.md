# zot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/patriceckhart/zot, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/zot

## Pinned environment

- Project commit: `f2fef94e4d0f93fefeda13562ac61cd352f5a4d2`
- Test commit: `f2fef94e4d0f93fefeda13562ac61cd352f5a4d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21.5 to 21.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 21.5 | 3 | 3 | [run](https://argusic.com/run/dd5bb80f-d44a-4f25-9a95-2592b3ad235e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go toolchain missing in container (no root to apt-install)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
