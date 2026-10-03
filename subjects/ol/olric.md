# olric

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/olric-data/olric, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/olric

## Pinned environment

- Project commit: `c49c44a8816b472943068b47916da9f26d15a349`
- Test commit: `c49c44a8816b472943068b47916da9f26d15a349`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 14.3 to 28.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 14.3 | 1 | 1 | [run](https://argusic.com/run/75127d30-6b5b-4264-b946-77e424b8033f) |
| 2 | pass | 100 | 13 | 14.8 | 0 | 0 | [run](https://argusic.com/run/fea70c6b-8cef-45cf-abdd-10dbc6c6127b) |
| 3 | pass | 100 | 28 | 28.5 | 2 | 2 | [run](https://argusic.com/run/c744cf2e-daae-4684-a475-218fd79555de) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go not found in container; Go 1.27.1 had compiler errors (redeclared symbols in internal/abi and crypto/internal/fips140)`

Attempt 3:

- 4 min: `Go compiler not installed`
- 6 min: `Go 1.25.0 pre-release had broken runtime (duplicate symbols in internal/abi and runtime)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
