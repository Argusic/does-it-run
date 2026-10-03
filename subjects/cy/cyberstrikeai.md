# CyberStrikeAI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AIPentest/CyberStrikeAI, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/cyberstrikeai

## Pinned environment

- Project commit: `470eb5ead185dc90f2441e89b31ceb1be913ac44`
- Test commit: `470eb5ead185dc90f2441e89b31ceb1be913ac44`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 16.6 | 1 | 1 | [run](https://argusic.com/run/066aaad7-60b5-41e7-a676-705d85f122fc) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.25.0 not found on system PATH (only Python 3.12.3 was pre-installed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
