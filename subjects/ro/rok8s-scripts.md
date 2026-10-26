# rok8s-scripts

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FairwindsOps/rok8s-scripts, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/rok8s-scripts

## Pinned environment

- Project commit: `ac1ab0db355b38b4965f9255a67150f23e7cdc2c`
- Test commit: `ac1ab0db355b38b4965f9255a67150f23e7cdc2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 4.1 | 1 | 1 | [run](https://argusic.com/run/52bc99b9-7f4c-4249-89ab-ff5c5fc7ae65) |

## What was observed on a clean machine

Attempt 1:

- `rm: cannot remove 'docker-credential-gcloud': No such file or directory (expected, gcloud not installed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
