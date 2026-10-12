# lazyrsync

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/westpoint-io/lazyrsync, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/lazyrsync

## Pinned environment

- Project commit: `e30d96b4c7d167b6db535931db2230afd619aa93`
- Test commit: `e30d96b4c7d167b6db535931db2230afd619aa93`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.4 to 31.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 31.4 | 4 | 4 | [run](https://argusic.com/run/ad119250-438a-449b-a2e4-387c4ec35863) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `no rustc/cargo in container`
- 3 min: `no rsync binary and no root for apt`
- 1 min: `TUI start panicked 'failed to initialize terminal' when launched without a TTY`
- 1 min: `driver sent literal backslash-r instead of Enter to the run-confirm dialog, so dialog input looked dead`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
