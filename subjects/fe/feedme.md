# FeedMe

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Seanium/FeedMe, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/feedme

## Pinned environment

- Project commit: `d3fcacf3504c6271470fdaada63c98cd9f79fa20`
- Test commit: `d3fcacf3504c6271470fdaada63c98cd9f79fa20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 5.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 5.8 | 3 | 3 | [run](https://argusic.com/run/039be52d-e3c3-4be1-bec8-282655524759) |
| 2 | pass with mocks | 92 | 15 | 10.8 | 4 | 4 | [run](https://argusic.com/run/418f4652-9abc-4daf-8f6d-106404ae80b3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 installed but project requires >=24`
- `Some external RSS feeds returned HTTP 429/403/503 (hnrss.org rate limit, linux.do blocked, rsshub.rssforever.com 503)`
- 2 min: `Mock LLM API server needed for summary generation (no real credentials)`

Attempt 2:

- 2 min: `Node.js 18.19.1 installed but project requires >=24.12.0; no version manager available to upgrade`
- 1 min: `update-feeds script uses .ts extension directly , Node 18 cannot execute TypeScript without a loader`
- 1 min: `Lockfile out of date with package.json; --frozen-lockfile failed`
- 2 min: `LLM API keys required for AI summary generation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
