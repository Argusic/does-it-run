# thanos

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thanos-io/thanos, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/thanos

## Pinned environment

- Project commit: `c1cba09dd1b175b0c8824f298f337b8092a47c05`
- Test commit: `c1cba09dd1b175b0c8824f298f337b8092a47c05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 17.7 | 3 | 3 | [run](https://argusic.com/run/07c5e08f-32b3-4818-b766-dfb24a9a5208) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in PATH`
- 2 min: `Tests panic with 'growslice: len out of range' due to wrong Labels implementation`
- 1 min: `Prometheus integration tests fail with 'executable file not found' for prometheus-v0.54.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
