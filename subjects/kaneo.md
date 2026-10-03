# kaneo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/usekaneo/kaneo, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kaneo

## Pinned environment

- Project commit: `6e47ef666d5f7b97a29d584112fa8e9a4f5c22a1`
- Test commit: `6e47ef666d5f7b97a29d584112fa8e9a4f5c22a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.9 to 26.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 26.9 | 6 | 6 | [run](https://argusic.com/run/75e47476-58e1-44fb-8e19-e13ca4d07cff) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (requires >=24)`
- 1 min: `pnpm not found`
- 8 min: `PostgreSQL not installed and no root apt/docker`
- 1 min: `npm global install failed due to /usr/local permissions`
- 1 min: `DATABASE_URL derivation requires POSTGRES_PASSWORD when POSTGRES_* vars are set`
- 1 min: `Integration tests require kaneo_test database`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
