# nimbus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sunchayn/nimbus, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/nimbus

## Pinned environment

- Project commit: `99c7822f88207b9dfa5e76fb4438e253ef8a9530`
- Test commit: `99c7822f88207b9dfa5e76fb4438e253ef8a9530`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.4 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 9.4 | 3 | 3 | [run](https://argusic.com/run/6e8a03c4-2cd2-498a-b5bc-bfff546a8183) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No PHP binary available in container; used FrankenPHP embedded PHP 8.5.12 CLI instead`
- 1 min: `No Composer binary available`
- `JS unit tests (vitest) fail because Node.js 18.19.1 is too old for vitest 4.x which requires Node 20+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
