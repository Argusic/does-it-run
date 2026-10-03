# TaxHacker

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vas3k/TaxHacker, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/taxhacker

## Pinned environment

- Project commit: `6cb7254b854b1f69c9e13775481e6aac79972424`
- Test commit: `6cb7254b854b1f69c9e13775481e6aac79972424`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 12.1 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 14 | 16.6 | 3 | 3 | [run](https://argusic.com/run/8700164d-91c5-4e35-ba0c-7f6d0791bd2b) |
| 2 | pass with mocks | 92 | 11 | 12.4 | 5 | 5 | [run](https://argusic.com/run/73827575-3888-4fc3-b20e-08dadf519316) |
| 3 | pass | 100 | 13.2 | 12.1 | 3 | 3 | [run](https://argusic.com/run/1249cca1-1483-485b-8119-2b1f064154e1) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18 found but project requires >=26. Installed v22.14.0 via prebuilt binary.`
- 5 min: `PostgreSQL not installed. Extracted postgresql-16 debs from Ubuntu archive.`
- 1 min: `Prisma adapter could not find libpq library at runtime.`

Attempt 2:

- 2 min: `Node.js v18 too old, requires >=26`
- 3 min: `PostgreSQL server not present`
- 1 min: `PostgreSQL failed to start: cannot create lock file in /var/run/postgresql, cannot bind IPv6`
- 0.5 min: `next binary not found on subsequent runs`
- 0.5 min: `App launched on port 3000 instead of configured PORT=7331`

Attempt 3:

- 2.5 min: `Node.js version 18 installed but project requires >=26`
- 5 min: `PostgreSQL not installed in container`
- 0.5 min: `PostgreSQL could not create lock file in /var/run/postgresql`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
