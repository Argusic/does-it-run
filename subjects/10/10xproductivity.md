# 10xProductivity

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ZhixiangLuo/10xProductivity, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/10xproductivity

## Pinned environment

- Project commit: `9a7da40bc798e4e3fe91b10770cf0fcc13cf0886`
- Test commit: `9a7da40bc798e4e3fe91b10770cf0fcc13cf0886`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.4 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 13.4 | 1 | 1 | [run](https://argusic.com/run/c40f7bbe-deed-4d3a-8fbc-1f980835bd12) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Slack integrations hardcode https://slack.com/api/*; local mock could not be intercepted because container DNS routes slack.com directly and /etc/hosts is not writable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
