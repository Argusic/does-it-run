# autopulse

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dan-online/autopulse, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/autopulse

## Pinned environment

- Project commit: `6c98b6beda76b6d7164ac790280d18aa93aa7db0`
- Test commit: `6c98b6beda76b6d7164ac790280d18aa93aa7db0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.3 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.5 | 11.5 | 0 | 0 | [run](https://argusic.com/run/ba1fb488-90ce-4d3b-a964-52168bfe8cf4) |
| 2 | pass | 100 | 16 | 7.3 | 1 | 1 | [run](https://argusic.com/run/93751aea-782a-40c0-b042-ca9a6de2e20e) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `cargo build default features failed: system libsqlite3 and libpq not found at link time`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
