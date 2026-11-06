# toydb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erikgrinaker/toydb, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/toydb

## Pinned environment

- Project commit: `0f42c9fc3b5cfc4327b7da95417459ef8a21a006`
- Test commit: `0f42c9fc3b5cfc4327b7da95417459ef8a21a006`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.3 to 16.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 16.4 | 2 | 2 | [run](https://argusic.com/run/ef8543b9-fa20-4f12-b257-929d415680a5) |
| 2 | pass | 100 | 2.5 | 6.3 | 1 | 1 | [run](https://argusic.com/run/f6494abc-2340-45df-88ce-e87ab3c88aa5) |

## What was observed on a clean machine

Attempt 1:

- `Rust not installed`
- `localhost resoles to IPv6 causing bind error 99`

Attempt 2:

- 2 min: `IPv6 not available: localhost resolves to ::1 which cannot bind/connect`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
