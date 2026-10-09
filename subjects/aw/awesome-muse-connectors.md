# awesome-muse-connectors

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Anil-matcha/awesome-muse-connectors, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/awesome-muse-connectors

## Pinned environment

- Project commit: `34d1378bac88e9cdd51a1400af6249692d6586f6`
- Test commit: `34d1378bac88e9cdd51a1400af6249692d6586f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 6.6 | 1 | 1 | [run](https://argusic.com/run/16ae7163-a8ae-4db5-87ff-035ba6034894) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing Muse runtime dependency (dynamic_credentials module at /opt/hatch/skills/skill-creator/bin/)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
