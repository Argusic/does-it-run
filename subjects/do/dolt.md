# dolt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dolthub/dolt, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/dolt

## Pinned environment

- Project commit: `4a2e8ce2f155f621cd904944c200ad356c758519`
- Test commit: `4a2e8ce2f155f621cd904944c200ad356c758519`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.4 to 28.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 28.4 | 2 | 2 | [run](https://argusic.com/run/ecb517e3-1325-4456-9ff0-6c2c4b24baca) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Source build failed: missing system libraries unicode/uregex.h (libicu-dev) and gozstd CGo bindings`
- `./sql.bats: 6 of 118 tests fail (tests #2, #18, #19, #20, #21, #23, #102, #110)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
