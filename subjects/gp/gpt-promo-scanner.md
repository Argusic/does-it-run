# gpt-promo-scanner

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JUk1-GH/gpt-promo-scanner, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gpt-promo-scanner

## Pinned environment

- Project commit: `be528fef2d59d2fc6d6d1abbd32a611df2c6fd86`
- Test commit: `be528fef2d59d2fc6d6d1abbd32a611df2c6fd86`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 43.2 to 43.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 43 | 43.2 | 2 | 2 | [run](https://argusic.com/run/486fd97c-6f90-4c15-9eeb-cfe932307b12) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `open_stripe.py hardcoded proxy http://127.0.0.1:7890 (closed in container) instead of using config/env proxy, always failing with curl(7) connect error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
