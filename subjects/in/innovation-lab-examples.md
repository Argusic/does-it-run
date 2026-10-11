# innovation-lab-examples

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fetchai/innovation-lab-examples, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/innovation-lab-examples

## Pinned environment

- Project commit: `ae840c28001b266a99e390e6e7d35cbe809b9f05`
- Test commit: `ae840c28001b266a99e390e6e7d35cbe809b9f05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 5.9 | 3 | 3 | [run](https://argusic.com/run/5af619f0-7950-4ca7-a6cf-8320c2f69436) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Orchestrator port 8003 already in use from previous run`
- `Almanac contract registration fails with insufficient funds (testnet)`
- `Orchestrator warns 'agent mailbox not found'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
