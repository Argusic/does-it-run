# temps

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gotempsh/temps, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/temps

## Pinned environment

- Project commit: `de626de659529233ce815a51d531d675cd14bc66`
- Test commit: `de626de659529233ce815a51d531d675cd14bc66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 85.4 to 85.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 75 | 85.4 | 4 | 4 | [run](https://argusic.com/run/287dc078-5aa0-4f74-91ad-9cdeb213962d) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System 'unzip' missing`
- 6 min: `pg_tsparser undefined symbol 'pg_atoi' (PG17 removed it)`
- 22 min: `Migrations failed: 'unrecognized parameter namespace timescaledb' on plain Postgres mock`
- 8 min: `web build failed on container Node 18 (Rspack needs 20.19+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
