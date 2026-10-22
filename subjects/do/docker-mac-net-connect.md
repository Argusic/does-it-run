# docker-mac-net-connect

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chipmk/docker-mac-net-connect, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/docker-mac-net-connect

## Pinned environment

- Project commit: `6039e2ba2cc3de5c8acd0ba77108dc94048b14db`
- Test commit: `6039e2ba2cc3de5c8acd0ba77108dc94048b14db`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 4 | 5.7 | 3 | 3 | [run](https://argusic.com/run/02463e73-10f7-48bc-b2c3-4aeae7a7e81a) |
| 2 | fail | 50 | 0 | 5.7 | 3 | 3 | [run](https://argusic.com/run/20f15fe8-ee9b-4eb6-8e9e-f4fd3f289928) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26.9 not installed (command not found)`
- 1 min: `GOROOT and GOPATH were the same directory causing warning`
- `Root module has '//go:build darwin' constraint, cannot compile natively on Linux`

Attempt 2:

- `Docker not available in container - cannot build Docker image or run e2e smoke test`
- `Host binary requires macOS (darwin build tag) - cross-compilation only on Linux`
- `make build fails because docker command is not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
