# fli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/punitarani/fli, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/fli

## Pinned environment

- Project commit: `881aee5ff4321e81ea2157cb44be94ce6a21dc1b`
- Test commit: `881aee5ff4321e81ea2157cb44be94ce6a21dc1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.6 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 7.6 | 2 | 2 | [run](https://argusic.com/run/ea37d7ce-558a-494f-92e6-d04c08124e90) |
| 2 | pass with mocks | 92 | 2 | 9.9 | 1 | 1 | [run](https://argusic.com/run/75f067ee-19cd-4024-820a-1d04b7033cb2) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not pre-installed`
- 3 min: `NO_COLOR=1 in container env causes Rich to skip hyperlinks, making test_display_date_results_links_dates_when_route_given fail`

Attempt 2:

- 4 min: `test_display_date_results_links_dates_when_route_given failed: Rich 14.1.0 sets color_system=None on StringIO even with force_terminal=True, suppressing OSC-8 hyperlink output`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
