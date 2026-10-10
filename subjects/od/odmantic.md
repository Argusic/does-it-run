# odmantic

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/art049/odmantic, licensed ISC, written in Python.

Evidence and recordings: https://argusic.com/subject/odmantic

## Pinned environment

- Project commit: `26e45046cfd780b0616abea25f0672de25a4a7dc`
- Test commit: `26e45046cfd780b0616abea25f0672de25a4a7dc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.5 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 12.5 | 5 | 5 | [run](https://argusic.com/run/a0ca31a1-564d-473a-83b3-eeae254ad279) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally-managed Python: system pip refused install`
- 4 min: `No MongoDB server available (no Docker, no mongod binary)`
- `Mongomock does not support $type:long/regex queries (8 test_type failures)`
- `Mongomock does not support $lookup with let/pipeline (10 reference failures)`
- `Mongomock has limited index support (14 index failures)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
