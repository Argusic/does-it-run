# resgate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/resgateio/resgate, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/resgate

## Pinned environment

- Project commit: `0cab702e09ff52306e59a3615d93eb29671a7f15`
- Test commit: `0cab702e09ff52306e59a3615d93eb29671a7f15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 3.7 | 4 | 4 | [run](https://argusic.com/run/f6112e1b-0657-4515-b75e-85e51cdd3355) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not found in container`
- 1 min: `NATS server not found`
- 1 min: `NATS server process died after shell command ended`
- 1 min: `Resolve of localhost to IPv6 when NATS only listened on IPv4`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
