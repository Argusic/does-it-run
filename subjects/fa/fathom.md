# fathom

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/usefathom/fathom, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/fathom

## Pinned environment

- Project commit: `2d895d8299d31c9957c806aa24720271668f3f09`
- Test commit: `2d895d8299d31c9957c806aa24720271668f3f09`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 6.6 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7.5 | 9.9 | 4 | 4 | [run](https://argusic.com/run/8ba83183-2732-46ad-853d-719c841cf3cb) |
| 2 | pass | 100 | 3 | 6.6 | 1 | 1 | [run](https://argusic.com/run/52e980d8-3cc0-47e8-8a87-966a5444d552) |
| 3 | pass | 100 | 25 | 21.9 | 2 | 2 | [run](https://argusic.com/run/07a46550-ab56-44da-98c9-2e9b4735e661) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `go not found`
- 2 min: `gcc not found (cgo requirement for sqlite3)`
- 0.5 min: `make not found`
- 1 min: `test binaries fail to exec (musl interpreter missing from /lib)`

Attempt 2:

- 1 min: `'go' binary not found in PATH; Go toolchain not installed`

Attempt 3:

- 3 min: `Go toolchain not installed in container`
- 35 min: `Referrer grouping never matched (Google/Bing/etc. always blank)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
