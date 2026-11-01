# Trend2Video-Pro

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/2417467487-hub/Trend2Video-Pro, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/62279d3b-f623-4d11-a452-7d4180ad3dfb

## Pinned environment

- Project commit: `ff224fc4bfb26b2a4bf53a871aecbace6de7ae75`
- Test commit: `ff224fc4bfb26b2a4bf53a871aecbace6de7ae75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 5.5 | 2 | 2 | [run](https://argusic.com/run/62279d3b-f623-4d11-a452-7d4180ad3dfb) |

## What was observed on a clean machine

Attempt 1:

- `Playwright browser not installed (chromium_headless_shell missing) - non-fatal, mock/fallback handles it`
- `Web fetch 403 on some URLs (e.g. ProductHunt) - non-fatal, pipeline uses fallback`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
