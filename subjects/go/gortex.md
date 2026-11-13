# gortex

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zzet/gortex, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gortex

## Pinned environment

- Project commit: `33107203de4900f1229a3eeff631ff9802c6725a`
- Test commit: `33107203de4900f1229a3eeff631ff9802c6725a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 68.7 to 75.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 68.7 | 3 | 3 | [run](https://argusic.com/run/33dbf063-fb4e-433f-9bee-77867754304b) |
| 2 | pass with mocks | 92 | 2.5 | 75.8 | 5 | 5 | [run](https://argusic.com/run/3996edfc-eaba-4603-aac6-119e63982763) |

## What was observed on a clean machine

Attempt 1:

- `internal/indexer tests: 9 watcher tests timed out (fsnotify events not delivered in container)`
- `internal/gitcmd: TestRunNoLazyNeverFetchesPromisedBlob fails , no promisor remote configured`
- `internal/gitstate: TestResolveViewSelectorPromisorObjectsNeverFetch fails , same promisor issue`

Attempt 2:

- 15 min: `gitcmd promisor tests fail: Git 2.43 returns exit 128 instead of 1 for failed lazy fetches, causing ObjectPresent() to abort rather than return false`
- 5 min: `gitstate TestResolveViewSelectorPromisorObjectsNeverFetch/missing_commit_tree fails: treeOfCommit() only checks exit 1, but Git 2.43 rev-parse returns 128`
- 30 min: `indexer/source TestGitTreeSourcePromisorObjectsNeverFetch/missing_root_tree and missing_blob_through_batch fail: resolveGitTreeOID and git cat-file batch both return 128 instead of 1`
- `store_sqlite times out after 10m in full test suite`
- `indexer times out after 10m in full test suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
