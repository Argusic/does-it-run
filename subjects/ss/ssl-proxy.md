# ssl-proxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/suyashkumar/ssl-proxy, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/ssl-proxy

## Pinned environment

- Project commit: `7cf7ab6b7bb433c013e0eefc00e95536a9248047`
- Test commit: `7cf7ab6b7bb433c013e0eefc00e95536a9248047`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 2 | 1 | 1 | [run](https://argusic.com/run/53b54038-392b-4a17-b75e-f2299be62c5f) |
| 2 | pass | 100 | 8 | 2.1 | 0 | 0 | [run](https://argusic.com/run/f0ff44f5-f932-4d5f-b316-9651adf34f75) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain not installed in container (no root to apt-install)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
