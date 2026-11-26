# browser-search

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Johell1NS/browser-search, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/browser-search

## Pinned environment

- Project commit: `398768aea1242506efdb8a3123b3a092602a6af0`
- Test commit: `398768aea1242506efdb8a3123b3a092602a6af0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.3 to 32.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 33 | 32.9 | 3 | 3 | [run](https://argusic.com/run/5234e511-8161-4686-b9bd-f5b0a89b81b3) |
| 2 | pass | 100 | 1.5 | 5.3 | 2 | 2 | [run](https://argusic.com/run/d0ad9888-6f7d-4aac-b1c5-8fd24381d80d) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Container Node.js is 18.19.1 but cloakbrowser/playwright-core require Node >=20 (runtime abort: 'Playwright requires Node.js 20 or higher')`
- 17 min: `Docker not installed and cannot be installed (no root); SearXNG and Camofox containers therefore cannot run`
- 5 min: `camofox.mjs health crashes when the API returns 503 (error thrown instead of recovering)`

Attempt 2:

- 0.5 min: `Node.js v18.19.1 is below the required >=20 for playwright-core@1.62.1`
- 0.5 min: `Docker is not available in this container so SearXNG and Camofox cannot run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
