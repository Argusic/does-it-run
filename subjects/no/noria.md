# Noria

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AhmadHassan-BTed/Noria, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/noria

## Pinned environment

- Project commit: `68a46c1e4402566ab5e54433d7d5e0aaba2d522a`
- Test commit: `68a46c1e4402566ab5e54433d7d5e0aaba2d522a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 11.3 | 2 | 2 | [run](https://argusic.com/run/5cb59b46-b7cb-4560-81fd-b96b23e58f81) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install failed: puppeteer postinstall tried to download Chrome but unzip is missing from the container (required by @puppeteer/browsers extraction)`
- 2 min: `pip3 install -r requirements.txt failed: externally-managed-environment (PEP 668) prevents system-wide pip install on Ubuntu 24.04`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
