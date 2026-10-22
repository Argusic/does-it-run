# sharelint

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jasonzhang06-source/sharelint, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sharelint

## Pinned environment

- Project commit: `910fa34ded16d4835f38f3e3a9470accea7dbb90`
- Test commit: `910fa34ded16d4835f38f3e3a9470accea7dbb90`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.5 to 1.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 1.5 | 1 | 1 | [run](https://argusic.com/run/a23ae4a4-dac9-4207-8ba8-2ebbf7b82d5d) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System pip refused install due to externally-managed-environment (PEP 668)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
