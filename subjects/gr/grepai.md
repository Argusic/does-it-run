# grepai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yoanbernabeu/grepai, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/grepai

## Pinned environment

- Project commit: `eb941fe8072b7a9af87e2604896456ae16a5127d`
- Test commit: `eb941fe8072b7a9af87e2604896456ae16a5127d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 5.5 | 1 | 1 | [run](https://argusic.com/run/caa2ece7-ee42-45be-a8d7-a402f4c26231) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.25.5 compiler not found in environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
