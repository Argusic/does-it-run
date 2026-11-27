# dayjs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iamkun/dayjs, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dayjs

## Pinned environment

- Project commit: `d3e43be0489ff1d010aca42b3115b6059215ed60`
- Test commit: `d3e43be0489ff1d010aca42b3115b6059215ed60`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.4 to 27.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 27.4 | 1 | 1 | [run](https://argusic.com/run/15d49adf-0f47-45eb-be47-6441fc526e7c) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `DST fall-back overlap test failed: dayjs.tz('2012-11-04 01:00', 'America/New_York') resolved to EST (-05:00) instead of EDT (-04:00). Root cause: in d.tz(), 'previousOffset' was computed as 'tzOffset(+d(), timezone)' using the current syste`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
