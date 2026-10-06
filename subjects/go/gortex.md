# gortex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zzet/gortex, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gortex

## Pinned environment

- Project commit: `33107203de4900f1229a3eeff631ff9802c6725a`
- Test commit: `33107203de4900f1229a3eeff631ff9802c6725a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 68.7 to 68.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 68.7 | 3 | 3 | [run](https://argusic.com/run/33dbf063-fb4e-433f-9bee-77867754304b) |

## What was observed on a clean machine

Attempt 1:

- `internal/indexer tests: 9 watcher tests timed out (fsnotify events not delivered in container)`
- `internal/gitcmd: TestRunNoLazyNeverFetchesPromisedBlob fails , no promisor remote configured`
- `internal/gitstate: TestResolveViewSelectorPromisorObjectsNeverFetch fails , same promisor issue`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
