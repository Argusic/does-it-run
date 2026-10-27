# broccoli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/besimple-oss/broccoli, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/broccoli

## Pinned environment

- Project commit: `6cad3b91b3bda89c7517326fc3b598c73949b04e`
- Test commit: `6cad3b91b3bda89c7517326fc3b598c73949b04e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42.2 to 42.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 42.2 | 1 | 1 | [run](https://argusic.com/run/ad81a11b-4312-4ac5-bafb-c66990e73209) |

## What was observed on a clean machine

Attempt 1:

- `14 integration tests fail when run against real Postgres because test code uses row[0] (list-style) while Database.connect sets dict_row. Pre-existing bug, not introduced by setup.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
