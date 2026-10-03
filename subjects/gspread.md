# gspread

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/burnash/gspread, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gspread

## Pinned environment

- Project commit: `7ca71eaa4658320b89f82f49620dac6891986cdd`
- Test commit: `7ca71eaa4658320b89f82f49620dac6891986cdd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 2 to 47.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.05 | 2 | 0 | 0 | [run](https://argusic.com/run/ae05ae78-5306-46cd-86ab-080dba7a528c) |
| 2 | pass with mocks | 92 | 0.3 | 3.8 | 0 | 0 | [run](https://argusic.com/run/924db2dc-7576-4e8a-8630-f7a0186a71b6) |
| 3 | pass with mocks | 92 | 4 | 47.5 | 2 | 2 | [run](https://argusic.com/run/da1e7246-acaf-4847-ba45-84871833005f) |

## What was observed on a clean machine

Attempt 3:

- 42 min: `requests 2.34.2 installed in a new venv redirects googleapis hostname resolution in ways that blocked my first local mock approach (DNS rewrite + adapter rewrite variants hit refused port 443); resolved by patching socket.getaddrinfo in the`
- 30 min: `Local mock's values-endpoint range parser crashed on gspread's %27Sheet1%27!A1%3A1 and row/col-range forms (A1:1, A1:A), closing connections; fixed expand_labeled normalization and added majorDimension=COLUMNS transposition`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
