# tntsearch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/teamtnt/tntsearch, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/tntsearch

## Pinned environment

- Project commit: `15191a83df525453ab310bbfb6b5097487d32692`
- Test commit: `15191a83df525453ab310bbfb6b5097487d32692`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.2 to 21.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 21.2 | 2 | 2 | [run](https://argusic.com/run/7554714b-5e19-4004-a38a-70b4d099a16b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `TNTGeoSearchTest::testFindNearestAtExactIndexedLocationIsReturned failed: PDO returned doc_id as string but assertContains uses strict identity`
- 8 min: `6 TNTIndexerTest tests + 1 TNTSearchTest failed: RedisEngine connection refused (no Redis server in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
