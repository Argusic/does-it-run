# go-proxmox

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/luthermonson/go-proxmox, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/go-proxmox

## Pinned environment

- Project commit: `f9f8ec1c961caca60dcf02adcabda7cb2b5d6530`
- Test commit: `f9f8ec1c961caca60dcf02adcabda7cb2b5d6530`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.9 to 17.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 17.9 | 2 | 2 | [run](https://argusic.com/run/727779ee-7e99-4116-8cdf-145c8dd76d5f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go 1.25 compiler not installed`
- 5 min: `Go standard library source not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
