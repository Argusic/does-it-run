# ferret

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MontFerret/ferret, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ferret

## Pinned environment

- Project commit: `5238ed795fe83ee76ca359b9e7bec6b9db2ffc05`
- Test commit: `5238ed795fe83ee76ca359b9e7bec6b9db2ffc05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.4 | 1 | 1 | [run](https://argusic.com/run/e60cf9cd-8c5f-4ccd-b3c5-438d0eafce74) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container , no go binary on PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
