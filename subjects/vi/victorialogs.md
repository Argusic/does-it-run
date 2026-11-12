# VictoriaLogs

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/VictoriaMetrics/VictoriaLogs, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/victorialogs

## Pinned environment

- Project commit: `bd02ecb1a13f736996c36bdd5d785a35d078c068`
- Test commit: `bd02ecb1a13f736996c36bdd5d785a35d078c068`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 1.6 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 8.5 | 0 | 0 | [run](https://argusic.com/run/b4086de6-e149-40ee-af80-a8aa10beadb5) |
| 2 | fail | 20 | n/a | 1.6 | 0 | 0 | [run](https://argusic.com/run/546b14e0-e215-4822-892d-9c5002b65847) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
