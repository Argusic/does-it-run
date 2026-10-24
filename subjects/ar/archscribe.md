# Archscribe

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lazypay/Archscribe, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/archscribe

## Pinned environment

- Project commit: `46ea42cfc6c557ab238867c390bb18320fd36769`
- Test commit: `46ea42cfc6c557ab238867c390bb18320fd36769`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 4.5 | 2 | 2 | [run](https://argusic.com/run/c354c482-83fb-48c0-b2ad-e772f4295457) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install -r requirements.txt failed: PEP 668 externally-managed environment, no root`
- 4 min: `2 browser tests skipped: playwright/rough.js unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
