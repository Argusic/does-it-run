# mcp-grafana

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/grafana/mcp-grafana, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/mcp-grafana

## Pinned environment

- Project commit: `7daeec61af208fb4f0aa18365aa0a5144bfd8d90`
- Test commit: `7daeec61af208fb4f0aa18365aa0a5144bfd8d90`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.4 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1 | 8.8 | 1 | 1 | [run](https://argusic.com/run/884127c2-499a-4822-a817-a66fd8e2ad7e) |
| 2 | pass | 100 | 7 | 7.4 | 0 | 0 | [run](https://argusic.com/run/a32e5599-bfb0-4df0-b93f-439581d66863) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
