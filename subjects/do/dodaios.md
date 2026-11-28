# Dodaios

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Dodaios/Dodaios, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/dodaios

## Pinned environment

- Project commit: `0664cee16ead61b9a21c1505b795fffa21216f13`
- Test commit: `0664cee16ead61b9a21c1505b795fffa21216f13`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39.4 to 39.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 39.4 | 5 | 5 | [run](https://argusic.com/run/fc87a28f-ffcb-43d0-8469-5c784a7a56d1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Headless server crash: PermissionError on /work/jarvis-agent-outputs because JARVIS_DATA_DIR was not set`
- 1 min: `Missing twilio module required by telephony tests`
- 1 min: `Missing mss module required by vision tests`
- 5 min: `Frontend npm run build OOM in memory-constrained container (~755MB RAM); Node 18 TSC + Vite needs >512MB`
- `tkinter not available (no root to apt-get install python3-tk)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
