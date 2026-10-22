# next-ecommerce

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RafaelGoulartB/next-ecommerce, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/next-ecommerce

## Pinned environment

- Project commit: `42630219b6ba41b79a64882d9772d21eb83753aa`
- Test commit: `42630219b6ba41b79a64882d9772d21eb83753aa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 5.2 | 3 | 3 | [run](https://argusic.com/run/c04f154b-44b1-4bd6-acdd-37355c00e260) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn is not installed in the container (README install step uses yarn)`
- 1 min: `next build exit code misread as failure because sh lacks ${PIPESTATUS}`
- 1 min: `npm run start with NODE_ENV=production returns connect ECONNREFUSED 127.0.0.1:3306 on authenticated mutations, because knexfile production config points at an unconfigured MySQL host`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
