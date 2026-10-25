# ioBroker.javascript

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ioBroker/ioBroker.javascript, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/iobroker-javascript

## Pinned environment

- Project commit: `365fc600a9a49826ce5314db9ddaac66abc1e7cf`
- Test commit: `365fc600a9a49826ce5314db9ddaac66abc1e7cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 10.1 | 2 | 2 | [run](https://argusic.com/run/1d422fe3-5518-4cb8-96ea-66df2261d986) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old (requires >=22.19.0)`
- 1 min: `src-editor npm install failed due to peer dependency conflict (jsdom@30 vs blockly@13 requiring jsdom@>=27.4.0 <30.0.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
