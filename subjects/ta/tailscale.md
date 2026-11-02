# tailscale

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tailscale/tailscale, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/tailscale

## Pinned environment

- Project commit: `d229a06f9a4b2340f0749288df0ac4f6de223acd`
- Test commit: `d229a06f9a4b2340f0749288df0ac4f6de223acd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.5 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.5 | 0 | 0 | [run](https://argusic.com/run/355c4529-ba8f-489d-b075-4f718224b217) |
| 2 | pass | 100 | 3.5 | 17.5 | 2 | 2 | [run](https://argusic.com/run/22d8d920-6562-42fc-bd5b-c7335a3a9611) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Tests fail without IPv6: cmd/natc and net/udprelay tests fail when IPv6 is disabled`
- 2 min: `ssh/tailssh tests fail without ssh binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
