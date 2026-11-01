# xedit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rotbit/xedit, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/xedit

## Pinned environment

- Project commit: `1f745aaedf5f1c9004773736d680ca9c061236a2`
- Test commit: `1f745aaedf5f1c9004773736d680ca9c061236a2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.4 | 5 | 5 | [run](https://argusic.com/run/489bb4d4-2b13-4eb0-b9ce-cb52c63c4ccc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container Node v18.19.1 too old for Next.js 16 (needs >=20.9; EBADENGINE warnings)`
- 3 min: `No system PostgreSQL or Docker available`
- 1 min: `Embedded Postgres tar has no psql/createdb`
- 1 min: `next start fails with output: standalone (Next.js 16 breaking change)`
- 1 min: `EADDRINUSE addr already in use :3000 and HTTP 000 from stray background server processes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
