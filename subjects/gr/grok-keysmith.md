# grok-keysmith

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jia-Ethan/grok-keysmith, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/grok-keysmith

## Pinned environment

- Project commit: `d2c3201d9fad6ca677eba2cb6b2ce276bc934d7f`
- Test commit: `d2c3201d9fad6ca677eba2cb6b2ce276bc934d7f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 4.5 | 2 | 2 | [run](https://argusic.com/run/dfb8b782-fc65-469d-b979-bc4ee43d4482) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `pytest not found in system Python`
- 0.1 min: `fake_grok.py lacked execute bit for 'run' subcommand`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
