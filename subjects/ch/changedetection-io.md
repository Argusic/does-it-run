# changedetection.io

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dgtlmoon/changedetection.io, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/changedetection-io

## Pinned environment

- Project commit: `fd7c9db23e371803bf1892b827b03d9c9c946bcd`
- Test commit: `fd7c9db23e371803bf1892b827b03d9c9c946bcd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 47.7 to 76 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 47.7 | 0 | 0 | [run](https://argusic.com/run/b3bcb05c-353a-4bd8-ac42-de02be9ab529) |
| 2 | pass | 100 | 5 | 76 | 3 | 3 | [run](https://argusic.com/run/77f54410-2db3-4d92-a877-9edcf5b472b7) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `pytest-flask live server defaulted SERVER_NAME to localhost.localdomain which does not resolve in this container (NameResolutionError on /test-endpoint)`
- 6 min: `PDFToHTMLToolNotFound: command-line 'pdftohtml' tool was not found in system PATH (poppler-utils not installed, no root)`
- 1 min: `run_basic_tests.sh failed with ModuleNotFoundError: No module named 'loguru' when invoked with system python3`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
