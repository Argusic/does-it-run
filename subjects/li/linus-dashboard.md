# Linus-Dashboard

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Thank-you-Linus/Linus-Dashboard, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/linus-dashboard

## Pinned environment

- Project commit: `46172e00d841578cfebdf708e7d0744b1a6d9644`
- Test commit: `46172e00d841578cfebdf708e7d0744b1a6d9644`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8.5 | 8.5 | 2 | 2 | [run](https://argusic.com/run/d94993ac-ee1c-4d8b-81cf-d241fa205fb3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `aiohasupervisor==0.6.0 not on PyPI (max 0.3.3)`
- 1 min: `homeassistant==2026.4.0 requires Python >=3.13, container has 3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
