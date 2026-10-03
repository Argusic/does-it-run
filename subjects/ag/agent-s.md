# Agent-S

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/simular-ai/Agent-S, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-s

## Pinned environment

- Project commit: `3aa272d23d2994c7bbde1acbbe0ef8e8d06b8693`
- Test commit: `3aa272d23d2994c7bbde1acbbe0ef8e8d06b8693`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 4.5 | 2 | 2 | [run](https://argusic.com/run/c9254293-85fe-4333-94be-8c523a51c536) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `setup.py python_requires '<=3.12' incompatible with Python 3.12.3`
- 3 min: `mouseinfo requires system package python3-tk on Linux (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
