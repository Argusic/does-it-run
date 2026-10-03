# optillm

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/algorithmicsuperintelligence/optillm, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/optillm

## Pinned environment

- Project commit: `eaf171aa6da5682ba1014ef342556f40247f5b35`
- Test commit: `eaf171aa6da5682ba1014ef342556f40247f5b35`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 22.3 to 31.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 31.1 | 0 | 0 | [run](https://argusic.com/run/9dfc0a6c-e751-42b7-be61-d411dde58f59) |
| 2 | pass | 100 | 18.5 | 22.3 | 2 | 2 | [run](https://argusic.com/run/1c63620f-e508-474e-a701-ffdba81ed444) |

## What was observed on a clean machine

Attempt 2:

- 2.5 min: `mcp v2.2.0 missing mcp.client.websocket module`
- 0.5 min: `test_batching.py, test_reasoning_tokens.py can't find test_utils`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
