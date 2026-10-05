# gita

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nosarthur/gita, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gita

## Pinned environment

- Project commit: `062a5e1ed56cad9b5f81c63791cd4ab130f175d9`
- Test commit: `062a5e1ed56cad9b5f81c63791cd4ab130f175d9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 4.5 | 1 | 1 | [run](https://argusic.com/run/316bcee1-be24-431b-8bbb-7e5e4e2940c5) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `3 tests failed due to hardcoded repo name 'gita' when checkout dir is 'repo'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
