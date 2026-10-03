# helix-db

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HelixDB/helix-db, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/helix-db

## Pinned environment

- Project commit: `c753c9d572964da5a19efd6f17fd8a8a2a5e248d`
- Test commit: `c753c9d572964da5a19efd6f17fd8a8a2a5e248d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 51.3 to 55.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 55.6 | 0 | 0 | [run](https://argusic.com/run/ecb498fc-4c8c-40a7-ae9d-db76a677ca95) |
| 2 | pass | 100 | 51 | 51.3 | 0 | 0 | [run](https://argusic.com/run/6f83610d-752c-44db-83bb-1f10892dae0a) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
