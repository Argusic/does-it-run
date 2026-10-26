# memlayer

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/divagr18/memlayer, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/memlayer

## Pinned environment

- Project commit: `5e95f44061a867a5ac0caf53434240713d58b86a`
- Test commit: `5e95f44061a867a5ac0caf53434240713d58b86a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.5 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 15.5 | 2 | 2 | [run](https://argusic.com/run/d5732398-bf82-4ca5-8abe-da3ad30abb50) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pytest crashed on collection: test scripts with module-level 'exit(0)' or side-effect code raised SystemExit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
