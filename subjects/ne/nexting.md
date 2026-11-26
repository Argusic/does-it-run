# nexting

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Nexting-ai/nexting, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/nexting

## Pinned environment

- Project commit: `3acb2c1ec7affa84fda6e7acce76bace98cdb2ab`
- Test commit: `3acb2c1ec7affa84fda6e7acce76bace98cdb2ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 19.4 to 39.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 39.7 | 5 | 5 | [run](https://argusic.com/run/0ae1f13c-cdf4-468d-9313-69c54fe45d50) |
| 2 | pass with mocks | 92 | 18 | 19.4 | 2 | 2 | [run](https://argusic.com/run/733408cf-e385-43e5-b14f-86aa8d2ff511) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18 lacks Array.toSorted() needed by openclaw peer dependency postinstall script`
- 18 min: `Say/Sync dual-response architecture not implemented , WS text handler only made one AI call`
- 8 min: `Offline message queue missing , no /pending endpoint, no queued flag on sendToDevice`
- 5 min: `No fallback AI call path when gateway RPC is disconnected`
- 1 min: `server.callDeviceTool() not exposed on PinclawWsServer class`

Attempt 2:

- 3 min: `Node.js 18 installed but package requires Node.js 22+. The openclaw peer dependency uses .toSorted() which is only available in Node 20+`
- 15 min: `Test suite had 19 failures , processMessage only called gateway RPC (not available in test), missing Say/Sync architecture, missing pending message queue, missing fallback AI support, missing hw/mode/userText fields on agent messages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
