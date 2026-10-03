# songloft

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/songloft-org/songloft, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/songloft

## Pinned environment

- Project commit: `e7807ff96554fc243943badbacbfb44fb9a5e055`
- Test commit: `e7807ff96554fc243943badbacbfb44fb9a5e055`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13.4 to 15.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 13.4 | 3 | 3 | [run](https://argusic.com/run/911ad28a-73f2-4f45-a9c8-7a048e763ef0) |
| 2 | pass | 100 | 12 | 15.7 | 1 | 1 | [run](https://argusic.com/run/a57bf5b1-ad0d-4257-be3f-cc41bd122741) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `root package test fails without -tags lite due to missing embedded frontend assets (expected by design)`
- 2 min: `Background server process terminated intermittently (health checker or signal)`
- 0.5 min: `pkg/tag submodule not initialized at clone`

Attempt 2:

- 2 min: `pkg/tag submodule not initialized; go build failed with 'reading pkg/tag/go.mod: no such file or directory'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
