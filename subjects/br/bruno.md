# bruno

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/usebruno/bruno, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/bruno

## Pinned environment

- Project commit: `14fc6acebfd8010b8e21bb8c7f876616ea19436e`
- Test commit: `14fc6acebfd8010b8e21bb8c7f876616ea19436e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 13 to 68.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 67 | 68.4 | 2 | 2 | [run](https://argusic.com/run/25a9bd08-9124-4e64-bc89-eb4c69a5feb6) |
| 2 | fail | 20 | n/a | 13 | 0 | 0 | [run](https://argusic.com/run/6b679e41-a27a-4283-9538-696cddaf26eb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `entry.parentPath is undefined on Node 18 (bruno-sqlite generate)`
- 5 min: `crypto is not defined in worker threads (serialize-javascript via @rollup/plugin-terser)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
