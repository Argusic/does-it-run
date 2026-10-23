# vandium-node

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vandium-io/vandium-node, licensed BSD-3-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/vandium-node

## Pinned environment

- Project commit: `339062d4bb2727aa8a311a6acc3cedf57734982e`
- Test commit: `339062d4bb2727aa8a311a6acc3cedf57734982e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 3 | 2 | 2 | [run](https://argusic.com/run/59be0f17-9cd7-416d-87ad-a4acafa55f89) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `handler invoked without Lambda context: TypeError 'Cannot destructure property succeed of undefined' at lib/event_types/handler.js:39`
- 0.1 min: `minimal synthetic API Gateway event failed with TypeError reading 'onResponse' of undefined at lib/event_types/api/api_handler.js:254`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
