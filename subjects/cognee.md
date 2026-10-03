# cognee

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/topoteretes/cognee, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/cognee

## Pinned environment

- Project commit: `eb90d03740755f5252b8b12cce91fd09970f2d81`
- Test commit: `eb90d03740755f5252b8b12cce91fd09970f2d81`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.1 to 33.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 33.1 | 1 | 1 | [run](https://argusic.com/run/c8315360-c445-444a-a79f-91609aeccac6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `psycopg2 build failed: pg_config not found (needs libpq-dev system package, can't install without root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
