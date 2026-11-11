# nikola

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/getnikola/nikola, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nikola

## Pinned environment

- Project commit: `ca72840e3014c183c8525566fe93af38928c69a1`
- Test commit: `ca72840e3014c183c8525566fe93af38928c69a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.4 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.4 | 0 | 0 | [run](https://argusic.com/run/ce612d1c-dd86-44a8-ad26-c4cd6a800cee) |
| 2 | pass | 100 | 5 | 7.3 | 1 | 1 | [run](https://argusic.com/run/b1ffbf41-9460-4c74-86b3-d6eb278e424d) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Test failure: test_format_date_timezone expected '-0400' but got 'EDT' due to updated Babel/CLDR timezone formatting`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
