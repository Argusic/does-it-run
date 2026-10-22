# drone-cli

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/harness/drone-cli, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/drone-cli

## Pinned environment

- Project commit: `3c6e2027200dc136decede9704cdfdf63ba79152`
- Test commit: `3c6e2027200dc136decede9704cdfdf63ba79152`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 7 | 4.6 | 4 | 2 | [run](https://argusic.com/run/86dc0ff3-1a83-4698-a432-5952edb8de64) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `curl failed to write go.tar.gz to /work (root-owned dir, no write permission for runner)`
- 4 min: `mock server process was killed between exec commands (only shell children of the exec session persisted)`
- 1 min: `'drone exec' requires the Docker daemon (docker binary not present, no root to install)`
- 1 min: `'drone verify' subcommand does not exist in this version of the CLI`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
