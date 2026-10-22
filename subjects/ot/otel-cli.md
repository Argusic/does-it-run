# otel-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/equinix-labs/otel-cli, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/otel-cli

## Pinned environment

- Project commit: `8f86e487b5f5badc8a4de50f0108e04bb38a7b4d`
- Test commit: `8f86e487b5f5badc8a4de50f0108e04bb38a7b4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.3 to 2.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.3 | 1 | 1 | [run](https://argusic.com/run/8cd4f2b0-9d72-466e-943d-dea633f4daa4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
