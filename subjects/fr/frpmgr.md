# frpmgr

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/koho/frpmgr, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/frpmgr

## Pinned environment

- Project commit: `60bf3e051bb772d1f34e4705bdb6cdc1a63278dd`
- Test commit: `60bf3e051bb772d1f34e4705bdb6cdc1a63278dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 10.8 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 12.4 | 10.8 | 4 | 4 | [run](https://argusic.com/run/3d3e1a5b-3bf7-4c90-8331-bde720455c7b) |
| 2 | pass with mocks | 92 | 16 | 17.2 | 3 | 3 | [run](https://argusic.com/run/11529c97-3e3c-4027-b1bd-9aacb2855733) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go compiler not found in container`
- 0.5 min: `file_test.go TestSplitExt fails on Windows-style path on Linux`
- `go generate fails (windres/MingW not available)`
- `Main app requires Windows GUI toolkit and Windows syscalls, cannot run on Linux`

Attempt 2:

- 1 min: `Missing platform build constraint on Windows-only source file pkg/util/net.go`
- 1 min: `Go 1.25.0 compiler not pre-installed in the container`
- 1 min: `Web UI dist/ not built - embed.go pattern dist fails on cross-compile`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
