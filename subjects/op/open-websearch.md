# open-webSearch

**Verdict: runs with mocks.** Argusic Score 77 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Aas-ee/open-webSearch, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-websearch

## Pinned environment

- Project commit: `a61bc65fc5edbf76b98bb81990e390b751617d01`
- Test commit: `a61bc65fc5edbf76b98bb81990e390b751617d01`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.7 to 15.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 77 | 30 | 15.7 | 4 | 1 | [run](https://argusic.com/run/4b42145d-d04f-47ca-a2d9-c624d4219b7a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `playwright-core bootstrap.js calls process.exit(1) on Node < 20, killing test subprocesses before they run`
- 2 min: `test-bing-live.js: Bing HTTP scraping returns zero results from this environment`
- 1 min: `test-dialog-capture.js: requires Playwright with a real browser, which needs Node >= 20`
- 1 min: `test-article-fetch-live.js: HTTP 521 from target CSDN server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
