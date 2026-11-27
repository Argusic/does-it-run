# reveal.js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hakimel/reveal.js, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/reveal-js

## Pinned environment

- Project commit: `e240e175232fa2de660a02bc0d7bf5f655b159bb`
- Test commit: `e240e175232fa2de660a02bc0d7bf5f655b159bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 3.4 | 5 | 5 | [run](https://argusic.com/run/7c1eb47b-e5fa-447a-8077-287dd4295b03) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 is below the required >=22.12.0`
- 2 min: `Puppeteer Chrome browser not found at expected cache path`
- 1 min: `Chrome crashpad_handler binary lacked execute permission`
- `Chrome requires --no-sandbox in container (no root)`
- 1 min: `No unzip utility available for extracting Chrome archive`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
