# elasticsearch-dump

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elasticsearch-dump/elasticsearch-dump, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/elasticsearch-dump

## Pinned environment

- Project commit: `e8fb1ea24c3472b60640c4e2972a92b56a587d3b`
- Test commit: `e8fb1ea24c3472b60640c4e2972a92b56a587d3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 42.9 to 49.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 42.9 | 0 | 0 | [run](https://argusic.com/run/973e045a-24a8-49a5-980f-20989d1b4a12) |
| 2 | pass with mocks | 92 | 0.07 | 49.5 | 1 | 1 | [run](https://argusic.com/run/03616568-637f-412e-8aaa-fa4fabdbf139) |

## What was observed on a clean machine

Attempt 2:

- 106 min: `31 ES-dependent tests fail because the mock ES server cannot fully replicate Elasticsearch APIs (offset/limit scroll, searchBody filtering, analyzer/settings/mapping/alias/template CRUD, parent-child queries, big-int parsing, csv-import bul`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
