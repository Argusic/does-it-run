# heimdall

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dadrus/heimdall, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/run/fd3872a7-74ee-46fb-bb66-7c3dd0d6586e

## Pinned environment

- Project commit: `4e12733a8e35cd690030e3d4c62583e1a60331c8`
- Test commit: `4e12733a8e35cd690030e3d4c62583e1a60331c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.1 to 32.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 32.1 | 2 | 2 | [run](https://argusic.com/run/fd3872a7-74ee-46fb-bb66-7c3dd0d6586e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.3 not installed in container`
- `go test fails with 'couldn't initialize inotify: too many open files' for 5 packages (cmd/validate, internal/secrets/provider/pem, internal/secrets/provider/file, internal/secrets/provider/jwks, internal/rules/provider/filesystem) when run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
