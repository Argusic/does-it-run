# a-stock-data

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/simonlin1212/a-stock-data, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/a-stock-data

## Pinned environment

- Project commit: `f814dcfe209dd7958f4858f9d878d591ee85fb56`
- Test commit: `f814dcfe209dd7958f4858f9d878d591ee85fb56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 28.4 to 40 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 40 | 3 | 3 | [run](https://argusic.com/run/d7dc86f0-383f-42e0-bf4e-8d8dbc1a38fd) |
| 2 | pass | 100 | 12 | 28.4 | 3 | 3 | [run](https://argusic.com/run/bd1be1f0-3536-4a43-bcf1-4224c7630b3a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Python PEP 668 blocks pip install`
- 10 min: `SSE margin trading API hard-caps at 2000 records per page but reports 2002 total`
- 5 min: `CNI index site www.cnindex.com.cn unreachable (SSL handshake timeout)`

Attempt 2:

- 20 min: `SSE margin API now caps each page at 2000 rows while reporting total=2017, so the shipped single-page checker raised '上交所该日数据未发布或分页不完整'`
- 15 min: `st_stock_list raised 'ST 名单为空或代码重复' because eastmoney's risk-warning board now includes 195 BJ 920xxx stocks that also appear in the BJ universe list, creating duplicate codes`
- 12 min: `sse_e_interaction raised '回复时间认不出: 1分钟前' because SSE-e now emits relative timestamps (1分钟前/5小时前/昨天 14:31) for recent items`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
