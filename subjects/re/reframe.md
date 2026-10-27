# reframe

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reframe-hpc/reframe, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/reframe

## Pinned environment

- Project commit: `a72c713c7cac15d8bdd0960eafe59c022f94733d`
- Test commit: `a72c713c7cac15d8bdd0960eafe59c022f94733d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 5.1 | 3 | 3 | [run](https://argusic.com/run/4be72dc2-8a76-4a0d-9571-0f903dae466c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip 24.0 ignores [dependency-groups] so '.[dev]' install skipped dev tools`
- 1 min: `pytest rejected --timeout=600 (no pytest-timeout plugin)`
- `shell reported 'Bad substitution' from my ${PIPESTATUS} snippet`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
