# deep-project

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/piercelamb/deep-project, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/deep-project

## Pinned environment

- Project commit: `c5436d57feaf86f8d49fc31926312725252d47d3`
- Test commit: `c5436d57feaf86f8d49fc31926312725252d47d3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.8 | 1 | 1 | [run](https://argusic.com/run/85e2a7e6-b318-4229-96c9-0ebc2a869a0d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv binary not on PATH; tests using subprocess.run(['uv', ...]) failed with FileNotFoundError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
