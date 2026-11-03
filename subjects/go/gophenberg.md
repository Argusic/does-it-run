# gophenberg

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gopherium/gophenberg, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gophenberg

## Pinned environment

- Project commit: `a3dc0e85d4820b05ba355e5c9eec0b0e8e76b044`
- Test commit: `a3dc0e85d4820b05ba355e5c9eec0b0e8e76b044`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.7 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 16.7 | 6 | 6 | [run](https://argusic.com/run/72a5b7e5-3daa-44aa-915e-82da3a113bf3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.27.3 compiler not found in PATH`
- 1 min: `pnpm not installed and npm install -g failed due to permissions`
- 3 min: `Docker not available for PostgreSQL`
- 1 min: `initdb failed: libpq.so.5 not found`
- 2 min: `pg_ctl failed: could not create lock file and could not bind IPv6`
- 1 min: `psql not found (only server binaries extracted)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
