# grok-reg-tool

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FengZi1221/grok-reg-tool, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/grok-reg-tool

## Pinned environment

- Project commit: `d609705f536d652169cecec989ec9aaeb3199968`
- Test commit: `d609705f536d652169cecec989ec9aaeb3199968`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.1 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 16.1 | 4 | 4 | [run](https://argusic.com/run/1e3c8ec6-2b9e-49bf-90b8-205e925c7a63) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `python3 -m pip install --user -r register/requirements.txt blocked by PEP 668 (externally-managed-environment)`
- 5 min: `/usr/bin/chromium and /usr/bin/chromium-browser absent, so DrissionPage had no browser to launch`
- 6 min: `Registration round aborted with 'page was refreshed' when the OTP page reloaded between fill and click`
- 2 min: `Local server defaults pythonPath to /usr/local/bin/python3, which does not exist here`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
