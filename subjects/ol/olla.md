# olla

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thushan/olla, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/olla

## Pinned environment

- Project commit: `bb0612193168513a3696bd01db5aa49cb5db7f8d`
- Test commit: `bb0612193168513a3696bd01db5aa49cb5db7f8d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 5.9 | 1 | 1 | [run](https://argusic.com/run/43473baf-2355-4452-ba8f-48aaa5cfd719) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.24.13 binary not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
