# news-crawl

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/commoncrawl/news-crawl, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/news-crawl

## Pinned environment

- Project commit: `8c08c28f67f28c09976c8b10ac48a7a483845aca`
- Test commit: `8c08c28f67f28c09976c8b10ac48a7a483845aca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 68.9 to 68.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 68.9 | 5 | 5 | [run](https://argusic.com/run/c611878d-ff21-41fb-ba61-78fe069eb246) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `OpenSearch bulk response parse NPE (bir is null) in StatusUpdaterBolt`
- 2 min: `Search response NPE: TotalHits.relation was null`
- 8 min: `Aggregations parse failures: unknown field partition / Could not parse aggregation keyed as [partition]`
- 1 min: `Mock returned 501 for HEAD /status (index-existence check)`
- 3 min: `No system root; java/Hadoop native libs unavailable via PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
