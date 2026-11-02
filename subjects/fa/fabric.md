# Fabric

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/danielmiessler/Fabric, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/fabric

## Pinned environment

- Project commit: `177b3a9d284895c907d6eb3a64937d174add4cd5`
- Test commit: `177b3a9d284895c907d6eb3a64937d174add4cd5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 7.6 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.8 | 0 | 0 | [run](https://argusic.com/run/adacbf2c-e8eb-487b-b435-20bc2e9bd26e) |
| 2 | fail | 80 | 14 | 7.6 | 0 | 0 | [run](https://argusic.com/run/372bf072-3388-4a3b-b4b3-0bd67da9db59) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
