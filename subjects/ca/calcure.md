# calcure

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anufrievroman/calcure, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/calcure

## Pinned environment

- Project commit: `c529fe27c5901c219576a7a51464947d30150b87`
- Test commit: `c529fe27c5901c219576a7a51464947d30150b87`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 4.8 | 1 | 1 | [run](https://argusic.com/run/ef41bcd4-d160-4fbf-8361-aaa00e08e2aa) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `config_folder.mkdir(exist_ok=True) failed because parent ~/.config didn't exist , Python's mkdir does not create parent directories by default`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
