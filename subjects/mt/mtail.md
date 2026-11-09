# mtail

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/mtail, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/mtail

## Pinned environment

- Project commit: `4c7e0e1174ac1ead032efe28d86428bbbe0ae145`
- Test commit: `4c7e0e1174ac1ead032efe28d86428bbbe0ae145`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.6 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6.1 | 0 | 0 | [run](https://argusic.com/run/b39431a1-b158-4360-b7b1-08310a729a6c) |
| 2 | pass | 100 | 1.5 | 2.6 | 0 | 0 | [run](https://argusic.com/run/bd8f8fbc-5be5-4c25-9bb8-52246bb639b1) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
