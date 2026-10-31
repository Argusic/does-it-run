# clodfarm

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/matank001/clodfarm, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/clodfarm

## Pinned environment

- Project commit: `2c839ec97382ad5f5df5b6810b3f2334a940869e`
- Test commit: `2c839ec97382ad5f5df5b6810b3f2334a940869e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 23.8 to 30.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 23.8 | 0 | 0 | [run](https://argusic.com/run/d585c060-038a-41c3-8ca8-269a6e76e124) |
| 2 | pass | 100 | 8 | 30.2 | 1 | 1 | [run](https://argusic.com/run/5bd0ae95-4b3e-44cd-bad0-ac615c9d49f7) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `test_schedules_fire_once_per_due_time_on_any_box failed on Friday: cron '0 9 * * 1-5' fires on weekdays, adding a third unexpected item to the assertion`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
