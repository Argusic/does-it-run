# sshpiper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tg123/sshpiper, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/sshpiper

## Pinned environment

- Project commit: `9f098eb24da9c3b904e464d61e57277cc7f0c544`
- Test commit: `9f098eb24da9c3b904e464d61e57277cc7f0c544`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.6 | 1 | 1 | [run](https://argusic.com/run/28d518ff-8aa0-483f-bac1-fb2339b0d3dd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
