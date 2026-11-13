# open-webSearch

**Verdict: runs.** Argusic Score 88.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Aas-ee/open-webSearch, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-websearch

## Pinned environment

- Project commit: `a61bc65fc5edbf76b98bb81990e390b751617d01`
- Test commit: `a61bc65fc5edbf76b98bb81990e390b751617d01`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.8 to 15.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 77 | 30 | 15.7 | 4 | 1 | [run](https://argusic.com/run/4b42145d-d04f-47ca-a2d9-c624d4219b7a) |
| 2 | pass | 100 | 2 | 3.8 | 1 | 1 | [run](https://argusic.com/run/2515bac0-8b3e-495f-9b3f-6051c1a13610) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `playwright-core bootstrap.js calls process.exit(1) on Node < 20, killing test subprocesses before they run`
- 2 min: `test-bing-live.js: Bing HTTP scraping returns zero results from this environment`
- 1 min: `test-dialog-capture.js: requires Playwright with a real browser, which needs Node >= 20`
- 1 min: `test-article-fetch-live.js: HTTP 521 from target CSDN server`

Attempt 2:

- 3 min: `playwright-core bootstrap.js and coreBundle.js hard-block Node.js < 20 at import time, killing all tests and runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
