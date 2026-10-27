# agent-chrome-relay

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aindeev/agent-chrome-relay, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/agent-chrome-relay

## Pinned environment

- Project commit: `ca2f952c04b43351250114d41eee440bfe26aa26`
- Test commit: `ca2f952c04b43351250114d41eee440bfe26aa26`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.7 to 19.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19.2 | 19.7 | 1 | 1 | [run](https://argusic.com/run/12c16b0b-c48d-4639-b73c-4a456de8c7b1) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `lsof is not available on Linux; relay's caller() function could not find connecting process PIDs, causing all agent connections to be rejected with code 4003 (tests 4-7, 12 failed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
