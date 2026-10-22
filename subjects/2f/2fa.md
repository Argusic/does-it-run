# 2fa

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wuzf/2fa, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/2fa

## Pinned environment

- Project commit: `2c9ffadfc3a9da44f64c3e22f6de3b58f1b5b3df`
- Test commit: `2c9ffadfc3a9da44f64c3e22f6de3b58f1b5b3df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 12 | 13 | 1 | 0 | [run](https://argusic.com/run/db3afea5-6210-4ddd-8230-a4cab1f62053) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Wrangler CLI requires Node.js >=20.3.0, container has v18.19.1 , cannot start dev server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
