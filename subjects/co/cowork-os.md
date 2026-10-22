# CoWork-OS

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CoWork-OS/CoWork-OS, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cowork-os

## Pinned environment

- Project commit: `eff5d1262b8f80fce0de1cfc1b4e2304144c97ec`
- Test commit: `eff5d1262b8f80fce0de1cfc1b4e2304144c97ec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 28.1 to 71 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 28.1 | 0 | 0 | [run](https://argusic.com/run/23cfddd7-b956-4815-8619-8bc00c651a60) |
| 2 | pass | 100 | 2 | 71 | 5 | 5 | [run](https://argusic.com/run/ba9447b8-a58d-415a-86e8-a15c8b79db74) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `npm install failed on Node 18 with 'Invalid comparator: npm:node-fetch-native@1.6.7'`
- 25 min: `sqlite3 CLI binary missing, breaking local-control-plane-discovery and qa-eval-runner tests (spawnSync sqlite3 ENOENT)`
- 3 min: `executor-step-failures test failed cleaning a directory symlink: ERR_FS_EISDIR`
- 15 min: `Numbat runtime manifest missing so NumbatBinaryResolver/integration tests failed (Go toolchain unavailable)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
