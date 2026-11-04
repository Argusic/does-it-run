# thanos

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thanos-io/thanos, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/thanos

## Pinned environment

- Project commit: `c1cba09dd1b175b0c8824f298f337b8092a47c05`
- Test commit: `c1cba09dd1b175b0c8824f298f337b8092a47c05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.7 to 21.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 17.7 | 3 | 3 | [run](https://argusic.com/run/07c5e08f-32b3-4818-b766-dfb24a9a5208) |
| 2 | pass | 100 | 20 | 21.3 | 3 | 3 | [run](https://argusic.com/run/2e291359-7edc-48ef-b446-f75370f20003) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in PATH`
- 2 min: `Tests panic with 'growslice: len out of range' due to wrong Labels implementation`
- 1 min: `Prometheus integration tests fail with 'executable file not found' for prometheus-v0.54.1`

Attempt 2:

- 8 min: `Go toolchain missing (go: not found); README requires Go 1.26.x; no root to apt-install`
- 18 min: `make test-local: pkg/reloader TestReloader_ConfigRollback failed: create watcher: too many open files (fsnotify.NewWatcher EMFILE)`
- 4 min: `thanos query process exited when its spawning exec session ended, so gRPC store RPC verification first failed with connection refused on 127.0.0.1:19193`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
