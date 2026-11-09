# huashu-chrome

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alchaincyf/huashu-chrome, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/huashu-chrome

## Pinned environment

- Project commit: `84d5ee40532ca586650d3d5f78f3952d3061cd06`
- Test commit: `84d5ee40532ca586650d3d5f78f3952d3061cd06`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.1 | 1 | 1 | [run](https://argusic.com/run/5d93efa9-e312-43c0-a849-84ed56d89d03) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node 18 compatibility: WebSocket not a global, causing ReferenceError in 'doctor' command`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
