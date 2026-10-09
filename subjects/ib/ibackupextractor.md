# ibackupextractor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unixzii/ibackupextractor, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/ibackupextractor

## Pinned environment

- Project commit: `85fa09f1af88e9d01a12a1d35ea20db1b6c44a51`
- Test commit: `85fa09f1af88e9d01a12a1d35ea20db1b6c44a51`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.5 to 3.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 3.5 | 2 | 2 | [run](https://argusic.com/run/84927d60-f6a9-442a-aeb7-80869b98f71e) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `cargo: not found`
- 8 min: `linker error: unable to find library -lsqlite3`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
