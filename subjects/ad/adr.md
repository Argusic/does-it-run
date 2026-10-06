# ADR

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/uber/ADR, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/adr

## Pinned environment

- Project commit: `9117d8a79c61861599e1d4deffdfb244584bfcb1`
- Test commit: `9117d8a79c61861599e1d4deffdfb244584bfcb1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 11.1 | 3 | 3 | [run](https://argusic.com/run/4cdad965-7d40-43bd-8309-0c026972680d) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `uv not found in PATH`
- 3 min: `Python.h not found (annoy C extension build failed)`
- 2 min: `x86_64-linux-gnu/python3.12/pyconfig.h not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
