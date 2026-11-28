# kander

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dualface/kander, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/kander

## Pinned environment

- Project commit: `a3acae584140a2b9d567f49b42cd5da69b111918`
- Test commit: `a3acae584140a2b9d567f49b42cd5da69b111918`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 46.8 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/248f118d-d93b-49ec-9b33-e6eb7408ffbf) |
| 2 | pass | 100 | 3 | 46.8 | 4 | 4 | [run](https://argusic.com/run/2b3e7e1d-a07e-43f8-b3d7-91a37bf305ca) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go compiler not installed in container`
- 1 min: `Node.js v18 too old for TypeScript test imports (needs --experimental-strip-types)`
- `internal/fs TestPosixPrivateRuntimeCleanupNeverFollowsSymlink fails: tempdir cleanup of read-only locked file gets permission denied`
- `internal/board TestModelCompositeStates times out after 10 minutes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
