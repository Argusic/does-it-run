# CasaOS

**Verdict: runs with mocks.** Argusic Score 87 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/IceWhaleTech/CasaOS, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/casaos

## Pinned environment

- Project commit: `0d3b2f444ec0193193cf03eef6d43c6e35b0183e`
- Test commit: `0d3b2f444ec0193193cf03eef6d43c6e35b0183e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.7 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 15 | 12.7 | 8 | 6 | [run](https://argusic.com/run/ab1fd228-6143-4633-9f14-02a543bcabc9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Go compiler in container`
- 1 min: `No yarn package manager`
- 1 min: `UI submodule not checked out`
- 1 min: `go build failed: missing codegen packages`
- 1 min: `URL files had trailing newlines causing panic`
- 2 min: `No gateway service for management address`
- `TestPorts fails (empty port list in container)`
- `UI private npm packages return 404`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
