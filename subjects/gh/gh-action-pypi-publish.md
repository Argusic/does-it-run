# gh-action-pypi-publish

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pypa/gh-action-pypi-publish, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/gh-action-pypi-publish

## Pinned environment

- Project commit: `dc37677b2e1c63e2034f94d8a5b11f265b73ba33`
- Test commit: `dc37677b2e1c63e2034f94d8a5b11f265b73ba33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 5.3 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 8.5 | 0 | 0 | [run](https://argusic.com/run/75056f84-f59b-486b-9534-6aba3b30ca4d) |
| 2 | pass with mocks | 92 | 18 | 5.3 | 1 | 1 | [run](https://argusic.com/run/5c4229e4-a4c4-43fe-a58a-0d4488973336) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `PYTHONPATH unbound variable in twine-upload.sh under set -u`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
