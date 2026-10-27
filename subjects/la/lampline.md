# Lampline

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/C4rohan/Lampline, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/lampline

## Pinned environment

- Project commit: `004aa7184b60b91343db81b67208a5ccbea9c68a`
- Test commit: `004aa7184b60b91343db81b67208a5ccbea9c68a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.7 to 22.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 22.7 | 1 | 1 | [run](https://argusic.com/run/ff99acdd-3c17-458f-a8cb-8eb6457a984f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_calendar_free_times_and_booking: busy times hardcoded in UTC broke across DST transition on Nov 1 2026`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
