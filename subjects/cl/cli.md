# cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hetznercloud/cli, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/cli

## Pinned environment

- Project commit: `88350084112192df1317e3cc101419ddcb85c689`
- Test commit: `88350084112192df1317e3cc101419ddcb85c689`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.3 | 1 | 1 | [run](https://argusic.com/run/3253488b-fb5b-4a93-9126-3df817a706a3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain not installed in container (missing: go binary)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
