# open-spaces

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Anil-matcha/open-spaces, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/open-spaces

## Pinned environment

- Project commit: `c789f40ccbbfea83ade5107926c04a6241ceb6b1`
- Test commit: `c789f40ccbbfea83ade5107926c04a6241ceb6b1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 9.7 | 6 | 6 | [run](https://argusic.com/run/fe194726-0f2b-4468-8d52-9febf203f8e5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `SQLAlchemy missing from requirements.txt , import error on startup`
- 2 min: `session.py raises RuntimeError when DATABASE_URL is not set (no PostgreSQL available)`
- 1 min: `Missing __init__.py in app/api/ and app/api/routers/ prevents module import`
- 3 min: `SQLite does not support ALTER TABLE IF NOT EXISTS , startup migration crashes`
- 2 min: `Node.js 18.19.1 incompatible with Next.js 16 which needs >=20.9.0`
- 1 min: `TailwindCSS native bindings compiled for wrong Node version after reinstall`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
