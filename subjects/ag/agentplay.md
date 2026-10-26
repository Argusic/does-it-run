# agentplay

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Entelligence-AI/agentplay, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/agentplay

## Pinned environment

- Project commit: `3851f5b05bc8dca15476a644c1959c16d5572559`
- Test commit: `3851f5b05bc8dca15476a644c1959c16d5572559`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 3 | 4.8 | 1 | 0 | [run](https://argusic.com/run/3893724a-3a51-4c34-a220-b6f703af35f8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Viewer vitest tests fail: 'File is not defined' (Node 18 vs 22+ global File API) and 'ERR_REQUIRE_ESM' in jsdom/html-encoding-sniffer. Root cause: Node.js v18.19.1 < required >=22. The viewer itself builds and serves correctly; only the tes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
