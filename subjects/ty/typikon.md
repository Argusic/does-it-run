# typikon

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/auula/typikon, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/typikon

## Pinned environment

- Project commit: `d81a1a9e66e62e3e2915f870fbb20c93c89b1584`
- Test commit: `d81a1a9e66e62e3e2915f870fbb20c93c89b1584`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 5 | 9.5 | 1 | 0 | [run](https://argusic.com/run/c2fa3b8b-f961-4e85-ae2e-ad9036ff255a) |

## What was observed on a clean machine

Attempt 1:

- `test_live_server hangs indefinitely because handle_watch_command() starts a blocking file-watcher loop`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
