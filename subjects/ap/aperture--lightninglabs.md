# aperture

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lightninglabs/aperture, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/77661f91-b25b-4e7e-9dc6-4991dae34b84

## Pinned environment

- Project commit: `355c52d6bb9be420b779cca57a794a2c7bb85b12`
- Test commit: `355c52d6bb9be420b779cca57a794a2c7bb85b12`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.9 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 21.9 | 4 | 4 | [run](https://argusic.com/run/77661f91-b25b-4e7e-9dc6-4991dae34b84) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go 1.26+ not installed in container`
- 0.5 min: `SQLite 'out of memory (14)' error when opening DB`
- 1 min: `Config validation: authenticator had conflicting lndhost+passphrase and missing lnd TLS files`
- 0.5 min: `Prometheus and main server bound to same port (11010) causing silent crash`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
