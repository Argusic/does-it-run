# humanize

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/humanfia/humanize, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/humanize

## Pinned environment

- Project commit: `60cab7e69fbff07dd2968088df6a64c6e23accd6`
- Test commit: `60cab7e69fbff07dd2968088df6a64c6e23accd6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.5 to 25.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 2.3 | 25.5 | 3 | 0 | [run](https://argusic.com/run/2c0195c2-cb5f-42f8-a3e4-a798df5555d4) |

## What was observed on a clean machine

Attempt 1:

- `2 integration tests (test_tui_epics.py) timeout in Textual headless mode`
- `A few integration tests (test_tui_settings, test_tui_flows, test_tui_monitor) hang in headless environment and could not be tested`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
