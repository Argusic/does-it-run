# top-user-agents

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microlinkhq/top-user-agents, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/top-user-agents

## Pinned environment

- Project commit: `2301c1d09de413664602b79f2b2ace9a0e558901`
- Test commit: `2301c1d09de413664602b79f2b2ace9a0e558901`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 5 | 2.9 | 2 | 1 | [run](https://argusic.com/run/a330369d-2580-41d9-bfd6-fb378ef3aa5c) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `npm test crashed on system Node v18.19.1: ava 7 pulls string-width 8.3.0 whose /v regex flag needs Node >=20 ('SyntaxError: Invalid regular expression flags')`
- 8 min: `bin/get, bin/update, bin/flush need a live Redis at REDIS_UA_URI (ioredis: connect ECONNREFUSED 127.0.0.1:6379); container has no redis-server binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
