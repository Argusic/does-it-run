# CliRelay

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kittors/CliRelay, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/clirelay

## Pinned environment

- Project commit: `51817dab76368ec43c42c8e3884d3dc9dd17f18c`
- Test commit: `51817dab76368ec43c42c8e3884d3dc9dd17f18c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11 to 37.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 37.4 | 2 | 2 | [run](https://argusic.com/run/da0249b8-7018-47b2-b4e4-cfad09e81394) |
| 2 | pass | 100 | 10 | 11 | 3 | 3 | [run](https://argusic.com/run/b38ca5b8-dfc4-4d99-b5eb-949e86773d06) |

## What was observed on a clean machine

Attempt 1:

- 23 min: `App startup intermittently died with 'failed to create watcher: too many open files' (EMFILE from inotify_init1) hitting fs.inotify.max_user_instances=128 while the management-panel auto-updater raced startup; ~2 of 4 launches failed`
- 46 min: `Plain 'go test ./...' failed in internal/watcher with the same EMFILE because parallel packages collectively exceeded the 128 inotify-instance cap`

Attempt 2:

- 2 min: `Go compiler not pre-installed in container. The go.mod requires Go 1.26.`
- 1 min: `go-install only (golang-1.26-go) has incomplete stdlib , missing packages like math/rand, sync/atomic, compress/flate, etc., causing build failures.`
- 1 min: `Server launch failed with 'postgres dsn is required' , PostgreSQL and Redis are mandatory runtime dependencies and cannot be installed without root.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
