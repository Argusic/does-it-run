# offen

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/offen/offen, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/offen

## Pinned environment

- Project commit: `ec99082a37ffb5855bd84debfef227d41c7b403c`
- Test commit: `ec99082a37ffb5855bd84debfef227d41c7b403c`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13 to 38.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 37 | 38.2 | 6 | 6 | [run](https://argusic.com/run/bbe24165-6271-4a91-a006-ba9316769132) |
| 2 | pass | 100 | 15 | 13 | 2 | 2 | [run](https://argusic.com/run/11dc2eb3-35c4-4131-b143-32e79cfe94b4) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go 1.22 too old for go.mod requiring 1.25`
- 2 min: `No C compiler (gcc) for CGO-dependent go-sqlite3`
- 2 min: `Musl-linked test binaries could not execute (no musl ld)`
- 5 min: `Chromium browser missing 40+ shared libraries for mochify tests`
- 1 min: `Port 9876 already in use`
- 1 min: `pnpm lockfile not found`

Attempt 2:

- `go test -cover on packages with no test files fails with 'go: no such tool covdata' when module requires go 1.25 but go 1.22 is installed`
- `vault/index.js tests fail when no test server is running on port 9876 (iframe postMessage origin mismatch)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
