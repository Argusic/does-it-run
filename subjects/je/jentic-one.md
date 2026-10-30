# jentic-one

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jentic/jentic-one, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/jentic-one

## Pinned environment

- Project commit: `c8af96ea88a6b937464edf9e8b5ef4f86c7d8a47`
- Test commit: `c8af96ea88a6b937464edf9e8b5ef4f86c7d8a47`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34 to 34 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 34 | 6 | 6 | [run](https://argusic.com/run/d06e3887-6cfb-418e-963f-b296c08503db) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv tool missing; Python deps could not be installed`
- 2 min: `UI build crashed on bundled Node v18.19.1 (node:util lacks styleText)`
- 2 min: `Rolldown native binding not installed under Node 22.11 (engine needs >=22.12)`
- `Local integration tests default to Postgres (unavailable without Docker)`
- 1 min: `Playwright browser missing for UI browser tests`
- `1 of 2873 UI tests failed (SegmentedToggle pill width 64>0) under headless Chromium`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
