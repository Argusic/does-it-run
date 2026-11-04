# GenericAgent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lsdefine/GenericAgent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/genericagent

## Pinned environment

- Project commit: `e86ca723a9439acef38349180b33ee31f45e3388`
- Test commit: `e86ca723a9439acef38349180b33ee31f45e3388`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 2.5 to 28.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 2.5 | 0 | 0 | [run](https://argusic.com/run/06d9cbcc-1b32-498a-bbc6-cd2f9d6f1042) |
| 2 | pass with mocks | 92 | 1 | 28.7 | 6 | 6 | [run](https://argusic.com/run/d734eee8-8f8c-4847-a60a-aa1e83b0b883) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `README's uv-based install could not run because uv is not installed in the container`
- `/usr/bin/time is unavailable, so the first timed install command failed before running`
- 2 min: `launch.pyw failed because pywebview found neither GTK Python bindings nor Qt bindings`
- 3 min: `frontends/tui_v3.py exited 1 when stdin was not a TTY`
- 5 min: `Automated PTY input could not trigger the TUI submit handler because the harness escaped control characters, so it made no model request`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
