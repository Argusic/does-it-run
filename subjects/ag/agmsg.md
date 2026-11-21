# agmsg

**Verdict: runs.** Argusic Score 56.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fujibee/agmsg, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/agmsg

## Pinned environment

- Project commit: `f5a72deb477efb3cd667d232f4b23c93e2ea3fe9`
- Test commit: `f5a72deb477efb3cd667d232f4b23c93e2ea3fe9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 16.5 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 2 | 20.2 | 3 | 2 | [run](https://argusic.com/run/fe15706c-b360-4032-b1b6-aaaff1235662) |
| 2 | fail | 20 | n/a | 16.5 | 0 | 0 | [run](https://argusic.com/run/b7d3e0c4-88fa-4e91-92dc-481a155b7f0e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `sqlite3 CLI binary not on system PATH`
- 1 min: `bats test runner not installed`
- `test_node_resolve.bats test 2 fails - NVM version-manager node path detection fails in container without NVM`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
