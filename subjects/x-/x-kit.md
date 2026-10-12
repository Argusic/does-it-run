# x-kit

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xiaoxiunique/x-kit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/x-kit

## Pinned environment

- Project commit: `04b6901c882ebddf8377923340ecae989e16a330`
- Test commit: `04b6901c882ebddf8377923340ecae989e16a330`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 6.2 | 1 | 1 | [run](https://argusic.com/run/1a859531-6e36-4700-a84f-43400f47db27) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `x_client_transaction.get_ondemand_file_url() fails against current x.com homepage (ondemand.s.js regex no longer matches)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
