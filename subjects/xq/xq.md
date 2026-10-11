# xq

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sibprogrammer/xq, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/xq

## Pinned environment

- Project commit: `224e3aeccc94c56ec2b203aebe78e48c1126a763`
- Test commit: `224e3aeccc94c56ec2b203aebe78e48c1126a763`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 4.6 | 1 | 1 | [run](https://argusic.com/run/133b444b-db64-47b5-ba59-564c90dcac70) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
