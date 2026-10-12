# due

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dobyte/due, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/due

## Pinned environment

- Project commit: `806892f51b0bc933c986b645c933e079cdbe2e3b`
- Test commit: `806892f51b0bc933c986b645c933e079cdbe2e3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 10.1 | 6 | 6 | [run](https://argusic.com/run/463fbb50-060c-4627-89ba-546c3ceecacd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.27.2 was not installed in the container`
- 1 min: `sonic v1.14.2 has no build constraints for Go 1.27 (only go1.24 and !go1.26)`
- 1 min: `config_test.go and config/file/config_test.go failed: stat ./config: no such file or directory`
- 1 min: `lock_test.go: nil pointer dereference because no Maker was set`
- 1 min: `internal/transporter/gate/builder_test.go: dial tcp 127.0.0.1:49899: connection refused`
- 1 min: `internal/transporter/node/builder_test.go: dial tcp 127.0.0.1:49898: connection refused`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
