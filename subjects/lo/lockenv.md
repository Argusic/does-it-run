# lockenv

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/illarion/lockenv, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/lockenv

## Pinned environment

- Project commit: `d0ecc5574805dfc4fd562870e8d9ae67b0bde42d`
- Test commit: `d0ecc5574805dfc4fd562870e8d9ae67b0bde42d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 6 | 1 | 1 | [run](https://argusic.com/run/53dd830a-0feb-4c70-a4df-818fff2c790a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `os.Root type lacks WriteFile/ReadFile/MkdirAll methods in Go 1.24`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
