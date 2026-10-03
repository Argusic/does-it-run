# aliyunpan

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tickstep/aliyunpan, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/aliyunpan

## Pinned environment

- Project commit: `d05d19acd827ce8cc7e80a55211eb29a11ee9177`
- Test commit: `d05d19acd827ce8cc7e80a55211eb29a11ee9177`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.9 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 10.9 | 4 | 4 | [run](https://argusic.com/run/2fe6e3ff-8a36-4cc9-8221-4f09940015de) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go binary not found in container`
- 3 min: `panlogin tests crashed with nil pointer dereference connecting to localhost:8977`
- 2 min: `bolt_db_test.go TestBoltUltraFiles: nil pointer dereference walking non-existent hardcoded path`
- 2 min: `sync_db_test.go: multiple tests (TestLocalSyncDb, TestLocalGet, TestSyncDbAdd) crashed on hardcoded paths`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
