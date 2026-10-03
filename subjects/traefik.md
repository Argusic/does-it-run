# traefik

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/traefik/traefik, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/traefik

## Pinned environment

- Project commit: `f08964179357f5170d1bc515213b16e120d02e6d`
- Test commit: `f08964179357f5170d1bc515213b16e120d02e6d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.1 to 34.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 34.1 | 3 | 3 | [run](https://argusic.com/run/ea78f397-510b-4999-a56d-c0dae9ce45ac) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.26.x not found in PATH`
- 2 min: `Docker not available for WebUI build - make binary fails`
- 1 min: `git describe fails - no tags in shallow clone`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
