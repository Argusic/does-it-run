# Trend2Video-Pro

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JiayiLu2003/Trend2Video-Pro, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/cd079f61-c105-46e5-8d12-ccc12a611a0a

## Pinned environment

- Project commit: `ff224fc4bfb26b2a4bf53a871aecbace6de7ae75`
- Test commit: `ff224fc4bfb26b2a4bf53a871aecbace6de7ae75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.27 | 14.2 | 6 | 6 | [run](https://argusic.com/run/cd079f61-c105-46e5-8d12-ccc12a611a0a) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `streamlit: not found because the README assumes virtualenv activation`
- 0.2 min: `Streamlit first-run email prompt blocked startup without a TTY`
- 3 min: `Streamlit displayed raw agent-card HTML in the Execute section`
- 4 min: `30-second subtitle files had 23 cues with end times before start times and past 30 seconds`
- 3 min: `Video quality checks reported resolution and audio as valid based only on file size`
- 1 min: `Product Hunt fetch returned 403 and its screenshot timed out while updating topics`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
