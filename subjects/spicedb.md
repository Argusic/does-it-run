# spicedb

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/authzed/spicedb, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/spicedb

## Pinned environment

- Project commit: `9145a33f9a092d3420be8469cb88f5ac30b16bc2`
- Test commit: `9145a33f9a092d3420be8469cb88f5ac30b16bc2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.9 to 15.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 15 | 15.9 | 3 | 1 | [run](https://argusic.com/run/12a6c304-9361-48c1-85b8-377172e026da) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26 not installed in container`
- 5 min: `pkg/cmd tests fail: requires Docker for CockroachDB testcontainer (rootless Docker not found)`
- 5 min: `pkg/testutil/sdbtestcontainer tests fail: requires Docker for SpiceDB testcontainer (rootless Docker not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
