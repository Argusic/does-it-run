# tellery

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tellery/tellery, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tellery

## Pinned environment

- Project commit: `0f0e1d2587b4358906726fab92c4d7fd3709fe28`
- Test commit: `0f0e1d2587b4358906726fab92c4d7fd3709fe28`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.6 to 25.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 25.6 | 4 | 4 | [run](https://argusic.com/run/695471ec-5678-4a82-9f8d-e5510dbccab7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm peer dependency conflict: typeorm requires ioredis@^4 but project uses ioredis@^5`
- 3 min: `No PostgreSQL binary available in container`
- 2 min: `zhparser extension not available for PostgreSQL`
- 15 min: `Chinese text search fails with simple participle - reversed CJK word matching fails`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
