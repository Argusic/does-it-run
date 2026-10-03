# ag-ui

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ag-ui-protocol/ag-ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ag-ui

## Pinned environment

- Project commit: `b8ebd02c84a3a2757990da47aebf7c55b708b1ef`
- Test commit: `b8ebd02c84a3a2757990da47aebf7c55b708b1ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.6 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 2 | 15.6 | 1 | 0 | [run](https://argusic.com/run/45c18ae4-817c-483f-a5bb-73869542c67e) |

## What was observed on a clean machine

Attempt 1:

- `dotnet CLI not found , cross-language .NET test suite fails to build its TestServer`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
