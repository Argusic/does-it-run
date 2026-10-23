# Vocello

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PowerBeef/Vocello, licensed MIT, written in Swift.

Evidence and recordings: https://argusic.com/subject/vocello

## Pinned environment

- Project commit: `0472486e059e972cdbb498fe3f6f61a21d3cc002`
- Test commit: `0472486e059e972cdbb498fe3f6f61a21d3cc002`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 17 | 12.3 | 5 | 4 | [run](https://argusic.com/run/90fa36c1-be38-4d76-90ad-20269495b75a) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `shallow clone (1 commit) had no refs/heads/main; HEAD was detached, breaking dev status and 1 test`
- 8 min: `lsof is not installed, so build_cleanup.py refuses cleanup and 8 tests failed`
- 3 min: `Node 18 lacks node:util.styleText needed by rolldown/vite; rendered-contract test crashed`
- 1 min: `npm ci warned EBADENGINE under system Node 18 (website requires Node 20.19+ or 22.12+)`
- 2 min: `macOS-only Swift/Xcode app and MLX TTS runtime cannot build or run on Linux x86_64 (no swift toolchain, no Apple Silicon, no Metal)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
