# ticket-monitoring

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dengmeiluan/ticket-monitoring, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ticket-monitoring

## Pinned environment

- Project commit: `844c5e19dbfc785d423cf667024832c585315e2e`
- Test commit: `844c5e19dbfc785d423cf667024832c585315e2e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 43.6 to 43.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 60 | 43.6 | 1 | 1 | [run](https://argusic.com/run/63d8d285-3085-472e-9467-7b1403a3d41d) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `netstat command not found - web UI tests that start demo server failed at fixture setup with FileNotFoundError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
