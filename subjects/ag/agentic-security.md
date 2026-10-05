# agentic_security

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/msoedov/agentic_security, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agentic-security

## Pinned environment

- Project commit: `b9755a9ead2fc086faef9a714207ab3b2574c96b`
- Test commit: `b9755a9ead2fc086faef9a714207ab3b2574c96b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.8 to 18.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 18.8 | 7 | 7 | [run](https://argusic.com/run/607f882e-60d0-40c2-a308-be2918abfc75) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pyproject.toml required Python >=3.14 but only 3.12 available`
- 0.5 min: `Old-style except syntax except X, Y: not supported`
- 0.5 min: `UTF-8 BOM in 3 module files causing parse errors`
- 3 min: `Forward reference annotations fail without from __future__ import annotations on Python 3.12`
- 1 min: `Missing test packages: inline-snapshot, huggingface-hub, pytest-mock, pytest-asyncio`
- 0.5 min: `System test used raw uvicorn command not in PATH`
- 1 min: `scikit-learn 1.9.1 broke OneClassSVM predict via missing _effective_probability`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
