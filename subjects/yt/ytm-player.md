# ytm-player

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/peternaame-boop/ytm-player, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ytm-player

## Pinned environment

- Project commit: `45af0220d4b1d2752568f2636191320cd9ea1ed7`
- Test commit: `45af0220d4b1d2752568f2636191320cd9ea1ed7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 14 | 3 | 3 | [run](https://argusic.com/run/156272fc-43f6-4b83-a663-3f04e57209bc) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System Python 3.12 is externally managed (PEP 668) , pip install fails without a venv`
- 0.3 min: `Editable install in venv failed because hatchling was not yet installed`
- 0.2 min: `mpv system binary and libmpv are not available in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
