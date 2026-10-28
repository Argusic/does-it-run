# agent-purge

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ZiChuanLan/agent-purge, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/agent-purge

## Pinned environment

- Project commit: `629494c706b604f0f421f748e2c1e261bcc9c6c8`
- Test commit: `629494c706b604f0f421f748e2c1e261bcc9c6c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.3 | 2 | 2 | [run](https://argusic.com/run/b2372950-4bb7-4d1e-8c1a-9ea339b5fced) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing lib/templates/personas/ directory - neutral.md starter persona not auto-generated on first run`
- 1 min: `npm install -g requires root permissions (EACCES)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
