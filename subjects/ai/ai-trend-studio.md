# ai-trend-studio

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/developeryj1992/ai-trend-studio, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-trend-studio

## Pinned environment

- Project commit: `a0600e01e766de9e5c8cef5134abff1060d0faa9`
- Test commit: `a0600e01e766de9e5c8cef5134abff1060d0faa9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 3.4 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 3.4 | 0 | 0 | [run](https://argusic.com/run/06237fea-5f3a-47d8-9ac2-ae6a94fedb12) |
| 2 | pass | 100 | 0.5 | 5.5 | 3 | 3 | [run](https://argusic.com/run/b94a5557-9fc0-4e05-842c-b2410e64de16) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `System pip rejects editable install on this Debian container (PEP 668 externally-managed-environment)`
- 0.1 min: `run.sh and the project quick-start invoke ./run.sh but the file has no executable bit, so a fresh checkout gives Permission denied`
- 0.1 min: `POST /api/imports runs compact_space before the SRT/VTT timestamp check, so a real SRT payload is stored with timestamps and content_source=manual instead of cleaned subtitle content`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
