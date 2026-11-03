# dolt

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dolthub/dolt, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/dolt

## Pinned environment

- Project commit: `4a2e8ce2f155f621cd904944c200ad356c758519`
- Test commit: `4a2e8ce2f155f621cd904944c200ad356c758519`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 28.4 to 36.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 28.4 | 2 | 2 | [run](https://argusic.com/run/ecb517e3-1325-4456-9ff0-6c2c4b24baca) |
| 2 | pass | 92 | 15 | 36.7 | 5 | 3 | [run](https://argusic.com/run/2c49de8f-6243-4c0d-bbda-19695fe6394c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Source build failed: missing system libraries unicode/uregex.h (libicu-dev) and gozstd CGo bindings`
- `./sql.bats: 6 of 118 tests fail (tests #2, #18, #19, #20, #21, #23, #102, #110)`

Attempt 2:

- 3 min: `Go toolchain missing (go: not found)`
- 4 min: `cgo build failed: unicode/uregex.h not found (libicu-dev headers absent, no root)`
- 3 min: `link failed: cannot find -licui18n/-licuuc/-licudata (only versioned .so.74.2 libs present, no dev symlinks)`
- 2 min: `go test ./libraries/utils/gpg fails: gpg binary not found in $PATH`
- 2 min: `go test ./store/nbs/... killed with 'signal: killed' (container memory limit)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
