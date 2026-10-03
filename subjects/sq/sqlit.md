# sqlit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Maxteabag/sqlit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sqlit

## Pinned environment

- Project commit: `5ad4559778bf2d73bbe51d0515935a0245501b11`
- Test commit: `5ad4559778bf2d73bbe51d0515935a0245501b11`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.5 to 18.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 18.5 | 1 | 1 | [run](https://argusic.com/run/d9bc7e38-929a-4bc3-b646-75c511826015) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `test_detect_strategy_pip_user_fallback failed because SystemProbe picked up real system stdlib EXTERNALLY-MANAGED marker, causing the probe to return 'externally-managed' instead of 'pip-user'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
