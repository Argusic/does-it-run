# erda

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erda-project/erda, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/erda

## Pinned environment

- Project commit: `7195c3a774d577783ab834c60cb0a6480ba0300d`
- Test commit: `7195c3a774d577783ab834c60cb0a6480ba0300d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 38.9 to 38.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 39 | 38.9 | 3 | 3 | [run](https://argusic.com/run/126e2741-6509-4991-ac88-78a1fbea086f) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Go not installed in the container (go: not found)`
- 12 min: `erda-proto-go v1.4.0 local replace directory api/proto-go had 0 generated .go files, causing 'no required module provides package' on all erda-proto-go imports`
- 5 min: `erda-proto-go's dependency chain includes 'github.com/coreos/bbolt@v0.0.0-00010101000000-000000000000: invalid version: unknown revision 000000000000' from an old erda-infra, preventing resolution of nearly all packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
