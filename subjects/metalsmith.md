# metalsmith

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/metalsmith/metalsmith, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/metalsmith

## Pinned environment

- Project commit: `9190ff2b66f4d72c28f417ae4a29146f49af12de`
- Test commit: `9190ff2b66f4d72c28f417ae4a29146f49af12de`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.2 | 1 | 1 | [run](https://argusic.com/run/bc08cce0-2f61-4e10-a32d-784e87e2881d) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Test 'CLI > init > should error when git is not in $PATH' fails because node and git share /usr/bin in this container, so restricting PATH to node's dir never removes git`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
