# localthings

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mbillow/localthings, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/localthings

## Pinned environment

- Project commit: `9fb27d3e6452fad6b809ba6af6b068da90827f3f`
- Test commit: `9fb27d3e6452fad6b809ba6af6b068da90827f3f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 5.3 | 1 | 1 | [run](https://argusic.com/run/31024f8e-a0a6-41a8-9881-8ff6ee8637b5) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System has Python 3.12 but this project requires 3.13+; pyenv build failed due to missing zlib-dev headers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
