# google-news-scraper

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lewisdonovan/google-news-scraper, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/google-news-scraper

## Pinned environment

- Project commit: `e34e5776176345eb7864471fb10d419ea46e9cd5`
- Test commit: `e34e5776176345eb7864471fb10d419ea46e9cd5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.1 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 13.1 | 4 | 4 | [run](https://argusic.com/run/5b89fa5c-0cef-406a-932e-fe6d6fced479) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `File global not defined in Node 18 for undici@7 (cheerio dep)`
- 1 min: `rollup config uses ESM imports, fails on Node 18 CJS loading`
- 1 min: `@babel/runtime missing at test time`
- 5 min: `CJS bundle crashes at require-time because jsdom/readability are ESM-only deps statically imported`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
