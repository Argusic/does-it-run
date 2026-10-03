# lux

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iawia002/lux, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/lux

## Pinned environment

- Project commit: `dd00f6d258d80b6684a0b9402d7124e5c18ef42f`
- Test commit: `dd00f6d258d80b6684a0b9402d7124e5c18ef42f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.7 | 11.4 | 3 | 3 | [run](https://argusic.com/run/f43ee46c-5b24-4616-892f-fe00ef19f08b) |
| 2 | pass | 100 | 4.5 | 11 | 2 | 2 | [run](https://argusic.com/run/122e0b1a-50cf-4ce2-8099-a6c16f77bf0c) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Go 1.24 not installed`
- 0.1 min: `app/app.go:34: non-constant format string in color.Color.Sprintf`
- 0.2 min: `extractors/ixigua/ixigua.go:72: nil dereference on FindSubmatch result`

Attempt 2:

- 3 min: `Go not installed in container , downloaded go1.27.1 tarball manually`
- 1.5 min: `app/app.go:34: non-constant format string in call to color.Sprintf , vet/build failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
