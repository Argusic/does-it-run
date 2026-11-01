# silver-tourism-digital-twin

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Zhangweihui666/silver-tourism-digital-twin, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/silver-tourism-digital-twin

## Pinned environment

- Project commit: `0e7c8e98218868973277088160d0cd3ed3988194`
- Test commit: `0e7c8e98218868973277088160d0cd3ed3988194`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.1 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1.1 | 0 | 0 | [run](https://argusic.com/run/09839d19-ae6e-4ae9-87c9-ffe1ae4bd2cf) |
| 2 | pass | 100 | 20 | 5.5 | 2 | 2 | [run](https://argusic.com/run/0b28867f-10c9-41f5-88e8-3bb73e10c316) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Python path detection only checked Windows .venv/Scripts/python.exe; on Linux the .venv/bin/python path was never found, causing figures endpoint to fail with python not found`
- 5 min: `scientific_figures.py crashes with ValueError: All wedge sizes are zero when no agents have completed/exited (empty or edge-case snapshot)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
