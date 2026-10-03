# mafl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hywax/mafl, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mafl

## Pinned environment

- Project commit: `7090a1a29d7f920c72af83833e7cacb6592327ee`
- Test commit: `7090a1a29d7f920c72af83833e7cacb6592327ee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.1 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.7 | 14.6 | 0 | 0 | [run](https://argusic.com/run/c26a9e2d-05b8-4ae7-aa40-516a01e176aa) |
| 2 | pass | 100 | 6 | 12.1 | 1 | 1 | [run](https://argusic.com/run/8fcaab8b-61cd-4456-8a62-bcdf19947314) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `First build failed because stale .nuxt dist remained from a prior interrupted run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
