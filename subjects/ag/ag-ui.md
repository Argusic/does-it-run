# ag-ui

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ag-ui-protocol/ag-ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ag-ui

## Pinned environment

- Project commit: `b8ebd02c84a3a2757990da47aebf7c55b708b1ef`
- Test commit: `b8ebd02c84a3a2757990da47aebf7c55b708b1ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.4 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 2 | 15.6 | 1 | 0 | [run](https://argusic.com/run/45c18ae4-817c-483f-a5bb-73869542c67e) |
| 2 | pass | 100 | 2 | 14.4 | 1 | 1 | [run](https://argusic.com/run/e415ed45-e37b-4891-8fa9-d3ea28c3d209) |

## What was observed on a clean machine

Attempt 1:

- `dotnet CLI not found , cross-language .NET test suite fails to build its TestServer`

Attempt 2:

- 1 min: `Node.js v18 too old: tsdown/rolldown needs 'styleText' from node:util, only in Node 22+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
