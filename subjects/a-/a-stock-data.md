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
- Valid runs: 1; wall time 40 to 40 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 40 | 3 | 3 | [run](https://argusic.com/run/d7dc86f0-383f-42e0-bf4e-8d8dbc1a38fd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Python PEP 668 blocks pip install`
- 10 min: `SSE margin trading API hard-caps at 2000 records per page but reports 2002 total`
- 5 min: `CNI index site www.cnindex.com.cn unreachable (SSL handshake timeout)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
