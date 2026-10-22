# api-firewall

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wallarm/api-firewall, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/api-firewall

## Pinned environment

- Project commit: `8ed75e4ca7dc66998265a0cac3d32acd2f167211`
- Test commit: `8ed75e4ca7dc66998265a0cac3d32acd2f167211`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.3 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 14.3 | 3 | 3 | [run](https://argusic.com/run/bdfeeafd-583b-44c9-8c68-36800ce7c730) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not found in base image`
- 1 min: `PROXY mode startup failed: required field RequestValidation missing`
- 1 min: `API mode startup error: DB with schemas not loaded`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
