# clawcodex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentforce314/clawcodex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/clawcodex

## Pinned environment

- Project commit: `5c179396277dc1650a316895b112eef7d9e7a0ad`
- Test commit: `5c179396277dc1650a316895b112eef7d9e7a0ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 50.9 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 50.9 | 3 | 3 | [run](https://argusic.com/run/e09cc91c-83b1-433d-820f-8d8be3616b6e) |
| 2 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/73a10d4a-ced0-4efa-95b9-707c92d8608c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_sigint_during_prefetch_clean_exit flaked , 100ms delay sent SIGINT during module import before signal handler was installed, returning rc=-2 instead of 130`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
