# stronghold

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alichtman/stronghold, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/stronghold

## Pinned environment

- Project commit: `94abec58559ad23150c0ac75d3e60ae02e301f00`
- Test commit: `94abec58559ad23150c0ac75d3e60ae02e301f00`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 1.6 to 2.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 1.6 | 1 | 1 | [run](https://argusic.com/run/c7e72a5d-8338-43e1-a17d-ae88f5127612) |
| 2 | pass with mocks | 92 | 1.5 | 2.5 | 2 | 2 | [run](https://argusic.com/run/043faeab-e62b-4bbf-8089-2629ff48b7e8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `SyntaxWarning: 'is' with str literal on line 25 of stronghold.py`

Attempt 2:

- 0.3 min: `String comparison used 'is' instead of '==' on line 25, causing SyntaxWarning`
- 0.5 min: `sp.run() on line 332 passed entire command as single list element without shell=True, causing FileNotFoundError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
