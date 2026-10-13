# whiteboard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cracker0dks/whiteboard, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/whiteboard

## Pinned environment

- Project commit: `cb4f34d3fcfc311fad05a0af5b49b3692fc93aa7`
- Test commit: `cb4f34d3fcfc311fad05a0af5b49b3692fc93aa7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.4 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.75 | 11.4 | 5 | 5 | [run](https://argusic.com/run/3e8dd2a8-b33e-418a-a1e3-8033d4ce6afc) |

## What was observed on a clean machine

Attempt 1:

- 0.08 min: `babel-jest fails to require() @babel/core v8 (ESM-only) , transform {} bypass needed`
- 0.07 min: `Jest ESM loader doesn't support 'with { type: "json" }' import assertion`
- 0.05 min: `crypto global not exposed in Jest's EVM sandbox, uuid package fails at runtime`
- 0.35 min: `jsdom@30.0.1 requires Node >=22 (Node 18 in container), html-encoding-sniffer requires() ESM @exodus/bytes`
- 0.1 min: `Production server loadwhiteboard/getReadOnlyWid fail with globalThis.crypto undefined in Node 18 EVM`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
