# babybuddy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/babybuddy/babybuddy, licensed BSD-2-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/babybuddy

## Pinned environment

- Project commit: `87570d32c55bd787fcc08490566f805233516315`
- Test commit: `87570d32c55bd787fcc08490566f805233516315`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.4 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 11.4 | 1 | 1 | [run](https://argusic.com/run/7ce90072-24d3-4599-95f6-e998cd469331) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `6 babybuddy view tests fail when run together due to test_password_reset logging out and polluting subsequent tests in the same class`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
