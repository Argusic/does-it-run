# utask

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ovh/utask, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/utask

## Pinned environment

- Project commit: `8164f7987bbb85708e4fc7b29d41095d6aa303cf`
- Test commit: `8164f7987bbb85708e4fc7b29d41095d6aa303cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.8 to 15.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 15.8 | 3 | 3 | [run](https://argusic.com/run/dccc18c7-9e57-45b4-8054-7e4643f9d585) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Go compiler in container`
- 3 min: `No PostgreSQL in container`
- 5 min: `Test pollution: running all tests together fails because templates/functions persist across packages in shared DB`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
