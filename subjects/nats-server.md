# nats-server

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nats-io/nats-server, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/nats-server

## Pinned environment

- Project commit: `eb6f3a8c57867fcfc04e97a1b865a21646c82702`
- Test commit: `eb6f3a8c57867fcfc04e97a1b865a21646c82702`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.8 to 14.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.8 | 14.8 | 1 | 1 | [run](https://argusic.com/run/61376d35-0047-4048-a6fe-5611e8f0d22e) |

## What was observed on a clean machine

Attempt 1:

- `Syslog not available in container causes TestSysLogger failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
