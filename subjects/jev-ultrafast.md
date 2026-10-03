# jev-ultrafast

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/jev-ultrafast, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/jev-ultrafast

## Pinned environment

- Project commit: `1231850a0bf1a0c0341fe408ef1668dbbfdfac46`
- Test commit: `1231850a0bf1a0c0341fe408ef1668dbbfdfac46`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 7.6 | 3 | 3 | [run](https://argusic.com/run/162e9823-875b-41f0-85b8-8a648cbbea7e) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not found in PATH`
- 3 min: `No Chromium browser found in container`
- 4 min: `browser-harness ensure_daemon() failed to detect running Chrome`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
