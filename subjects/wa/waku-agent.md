# waku-agent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ShenSeanChen/waku-agent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/waku-agent

## Pinned environment

- Project commit: `12bf00efb11fe27ee2d456a144e96ea0414678b9`
- Test commit: `12bf00efb11fe27ee2d456a144e96ea0414678b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 7.1 | 1 | 1 | [run](https://argusic.com/run/5c1ffcd1-128a-49ac-8b3a-eecf4c93e1dd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `hosted extra dependency jwt (PyJWT) not installed, causing 4 collection errors in evals/deterministic/hosted/*.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
