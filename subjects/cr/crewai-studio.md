# CrewAI-Studio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/strnad/CrewAI-Studio, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/crewai-studio

## Pinned environment

- Project commit: `8b123b34624f06c1630465fa23e537b02ecaa6eb`
- Test commit: `8b123b34624f06c1630465fa23e537b02ecaa6eb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.9 | 1 | 1 | [run](https://argusic.com/run/7e9fcf84-e39e-4c0a-89fa-ade82629f07a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `requirements.txt does not include pytest, so the bundled tests cannot run after the standard install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
