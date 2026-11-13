# cli

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hetznercloud/cli, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/3253488b-fb5b-4a93-9126-3df817a706a3

## Pinned environment

- Project commit: `88350084112192df1317e3cc101419ddcb85c689`
- Test commit: `88350084112192df1317e3cc101419ddcb85c689`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.5 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.3 | 1 | 1 | [run](https://argusic.com/run/3253488b-fb5b-4a93-9126-3df817a706a3) |
| 2 | pass | 100 | 2 | 4.5 | 0 | 0 | [run](https://argusic.com/run/2369cf4f-03db-4765-a799-4c64eab0d2c4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain not installed in container (missing: go binary)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
