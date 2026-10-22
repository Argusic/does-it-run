# trends-checker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/akvise/trends-checker, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/trends-checker

## Pinned environment

- Project commit: `f8910793bda2035eee5e9fd7ab8a391c8d7bcb46`
- Test commit: `f8910793bda2035eee5e9fd7ab8a391c8d7bcb46`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 5.3 | 1 | 1 | [run](https://argusic.com/run/0207d5b5-0087-478b-bb93-b18d33192701) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pytrends 4.9.2 uses deprecated 'method_whitelist' keyword in urllib3 Retry(), which was renamed to 'allowed_methods' in urllib3 v2.x`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
