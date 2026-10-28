# dorabot

**Verdict: runs with mocks.** Argusic Score 78.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/suitedaces/dorabot, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dorabot

## Pinned environment

- Project commit: `ed7226ef32b06318307997fc59da66e2407ed548`
- Test commit: `ed7226ef32b06318307997fc59da66e2407ed548`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 28.9 to 28.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 78.67 | 1.2 | 28.9 | 3 | 1 | [run](https://argusic.com/run/9745e7d0-cadf-4c5c-b6c2-5f6c8ddd92cb) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 (pre-installed) does not meet project requirement of >=22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
